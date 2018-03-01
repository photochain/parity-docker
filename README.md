Parity in Docker
===

# Mainnet

```shell
docker-compose up mainnet
```

# Kovan

```shell
docker-compose up kovan
```

# Volume on external disk

Substitue `$YOUR_PATH` with absolute path to mounted disk

```shell
docker volume create --opt type=ext4 --opt device=$YOUR_PATH --opt o=bind --name parity_kovan
docker volume create --opt type=ext4 --opt device=$YOUR_PATH --opt o=bind --name parity_mainnet
```
