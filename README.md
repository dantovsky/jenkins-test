# Uploading files to Hosting Using Jenkins and git-ftp

## Baseado no vídeo e post:
- https://www.youtube.com/watch?v=ZdUk3UeG8JQ
- https://medium.com/@diegohyenna/usando-git-ftp-como-alternativa-de-deploy-2368ed33d9d5

## Config do vídeo para o Jenkins:
```
git config git-ftp.syncroot .
git ftp push --user $FTP_USERNAME --passwd $FTP_PASSWORD ftp://ftp.imediacto.com/jenkins.imediacto.com/
```

```
## Config passo-a-passo, seguindo orientações do post do Diego Guimarães:
git config git-ftp.syncroot .
git config git-ftp.user $FTP_USERNAME
git config git-ftp.url ftp://ftp.imediacto.com/jenkins.imediacto.com/
git config git-ftp.password $FTP_PASSWORD
git ftp push
```