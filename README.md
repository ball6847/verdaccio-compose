SIMPLE VERDACCIO COMPOSE FILE
=============================

After cloning or downloading this repository, you should change ownership of storage directory to (100:100) in order to make verdaccio work properly in docker

```sh
sudo chown -R 100:100 storage/
docker-compose up -d
```

Please note that the container will restart itself after reboot, so if you're just playing around, you can just remove the restart directive in `docker-compose.yml`

Setup Npm Registry
------------------

```sh
npm set registry http://localhost:4873
```
