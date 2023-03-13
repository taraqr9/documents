\*\*\* Remove changes all

```shell
git restore .
```

\*\*\* Remove changes from fileName.txt

```shell
git restore fileName.txt
```

\*\*\* Remove untracked file

##### To remove the untracked files you should first use command to view the files that will be affected by cleaning
```shell
git clean -fdn
```
##### This will show you the list of files that will be deleted. Now to actually delete those files use this

##### Now use this command to delete all untracked files

```shell
git clean -fd
```