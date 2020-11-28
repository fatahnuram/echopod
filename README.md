# echopod

Simple HTTP server that tells you the scheme, domain, and the URL path. It is just NGINX with custom config.

## How to run

Pull the image.

```bash
docker pull fatahnuram/echopod:latest
```

Run it.

```bash
docker run -d --name echopod -p 8080:80 fatahnuram/echopod:latest # running in background
# or
docker run --rm -p 8080:80 fatahnuram/echopod:latest # running in foreground
```

Test the connection.

```bash
curl localhost:8080
curl localhost:8080/somepath/tobe/checked
```
