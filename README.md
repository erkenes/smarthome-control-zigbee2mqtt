# smarthome-control-zigbee2mqtt

Start a MQTT and Zigbee2MQTT Server.

## Usage

Start the containers with

```shell
docker-compose up -d
```


Based on the instructions form [Zigbee2Mqtt](https://www.zigbee2mqtt.io/guide/getting-started/#installation)

## Services

### MQTT

Default user: mosquitto<br />
Default password: admin

To change the password (or the username), start the containers and run

```shell
docker-compose exec mosquitto mosquitto_passwd -c /mosquitto/config/mosquitto.passwd your_username

```

Replace `your_username`with the username you want to use. Remeber: All other user accounts will be replaced!

:warning: You need to replace the mqtt login data in the secret.yaml at the file: `Data/zigbee2mqtt/secret.yaml`
