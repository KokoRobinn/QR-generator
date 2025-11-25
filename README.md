# [WIP] QR code generator web app
This is a hobby project with the purpose of learning golang and the QR standard.
The code is therefore quite awful at the moment.

## Setup

Clone the repo and run:
```
docker build -t <USER>/qr src/
```
Then put the user you entered above in the docker-compose file, as well as the directory where you want your QR codes stored.
After running `docker compose up` you can access the app at port 1010.
