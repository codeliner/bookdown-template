## Generate Documentation

```bash
$ docker run -it --rm -e CSS_BOOTSWATCH=yeti -e CSS_PRISM=ghcolors -v $(pwd):/app sandrokeil/bookdown:develop docs/bookdown.json
$ docker run -it --rm -p 8080:8080 -v $(pwd):/app php:5.6-cli php -S 0.0.0.0:8080 -t /app/docs/html
```