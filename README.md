# questitto
Mosquitto + Telegraf + QuestDB Easy-to-Deploy Stack for quick IoT Prototype Scenarios using Docker

## Components

### QuestDB
- UI available on port `http://localhost:9000`
- TCP/ UDP port on `tcp://localhost:9009` or `udp://localhost:9009`

### Mosquitto
- Minimal configuration to provide logs on `stdout` for `docker-compose logs`
- available on `tcp://localhost:1883`
- Add / Remove users in `mosquitto/config/passwd` file

### Telegraf
- based on [TIG Stack example in tiguitto](https://github.com/shantanoo-desai/tiguitto) the configuration remains same
- See / Adapt the `topics` array in the `telegraf.conf` file
- Remove / Adapt the `processors.regex` and `processors.enum` configuration in `telegraf.conf`


## Blog Post

Complete write up [here](https://shantanoo-desai.github.io/posts/technology/questitto_light_stack_for_iot/)