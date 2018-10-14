# HOWTO

```bash
docker build -t erd .
docker run -v $(pwd):/home erd -i /home/file.er -o /home/file.pdf
```