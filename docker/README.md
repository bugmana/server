# HOW TO START


## Create the working space
```
mkdir mangosone
cd mangonsone
```
Clone frome the official repo
```
git clone https://github.com/mangosone/server.git . --recursive --depth=1
```

Create the folder `/mangosone/mangos` for bin, etc, game data (maps, vmaps, mmaps, dbc) folders/files
```
mkdir mangos
cd mangos
mkdir bin etc
```

Create folder `/etc/mangosd_conf` and `/etc/realmd_conf` which will hold the backup configuration files `mangosd.conf.dist` and `realmd.conf.dist`
```
cd etc
mkdir mangosd_conf realmd_conf
```

## Build docker images and generate config files and tools
Go to the docker files
```
cd /mangosone/server/docker
```

Please view and/or edit the `docker-compose.yml` file, then execute
```bash 
docker-compose.yml up --build
```
This will generate 
- Config files `mangosd.conf.dist`, `realmd.conf.dist` 
- 
