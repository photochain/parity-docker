Parity in Docker container
===

# Mainnet

```shell
docker-compose up mainnet
```

# Kovan

```shell
docker-compose up kovan
```

# Custom volume location (e.g. external disk)

Substitue `$YOUR_PATH` with absolute path

```shell
docker volume create --opt type=ext4 --opt device=$YOUR_PATH/parity_kovan --opt o=bind --name parity_kovan
docker volume create --opt type=ext4 --opt device=$YOUR_PATH/parity_mainnet --opt o=bind --name parity_mainnet
```
