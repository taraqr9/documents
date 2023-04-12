\*\*\* add a enum class

```shell
enum ClassName: string {
    case ONE = '1';
    case TWO = '2';
}
```

\*\*\* get values from enum

```shell
ClassName::ONE  

<-- 
This will return a array, So the output is 

ClassName Enum:int
(
    [name] => ONE
    [value] => 1
)
-->


ClassName::ONE->name 
<-- 
OUTPUT

ONE
-->

ClassName::ONE->value 
<-- 
OUTPUT

1
-->
```

\*\*\* get reverse value

```shell
ClassName::from('1')->name
<-- 
OUTPUT

ONE

********* This will print name, not value.
-->
```

\*\*\* This will print all value inside class.

```shell
@foreach(\App\Enums\ClassName::cases() as $blood)
    <option value="{{$blood->value}}">{{$blood->name}}</option>
 @endforeach

<--
********* This will also return the same array.
-->
```
