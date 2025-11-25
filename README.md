# [WIP] QR code generator web app
This is a hobby project with the purpose of learning golang and the QR standard.
The code is therefore quite awful at the moment.
In its current state it does not add data padding, ECC or masking to the code and thus does not produce a valid code.
When those features are implemented, it will be able to produce V3 codes with byte encoding with L-level ECC and variable masks.
Making it support all QR versions and ECCs will likely take a while.

## Setup

Clone the repo and run:
```
docker build -t <USER>/qr src/
```
Then put the user you entered above in the docker-compose file, as well as the directory where you want your QR codes stored.
After running `docker compose up` you can access the app at port 1010.
