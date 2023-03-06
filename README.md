# Whisper-UI Docker-Image
Docker image for [whisper-ui](https://github.com/hayabhay/whisper-ui)

### Docker CLI example
```sh
docker run -d \
  --name whisper-ui \
  --restart unless-stopped \
  --device=/dev/dri:/dev/dri \
  -p 8298:8501 \
  -e TZ=Europe/Bucharest \
  -v /home/radu/.whisperui:/data \
  ghcr.io/rursache/whisper-ui-docker-image:latest
```
