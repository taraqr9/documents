\*\*\* Expose a web server on port 80 of your local machine to the internet

```
ngrok http 80
```
\*\*\*  Expose a secure web server on port 5001 of your local machine to the internet

```
ngrok http https://localhost:5001
```

\*\*\*  Open a tunnel with the subdomain 'inconshreveable'

```
ngrok http -subdomain=inconshreveable 80
```

\*\*\*  Password-protect your tunnel

```
ngrok http -auth="username:password" 8080
```

\*\*\*  Forward to an https server by specifying the https:// scheme

```
ngrok http https://localhost:8443
```

\*\*\*  Forward to the default https port on localhost

```
ngrok http 443
```