# elk

elk is a docker compose file for dealing with elasticsearch world (logstash, elasticsearch, kibana). Support both arm64 and amd64

## Installation

Just clone this repo.

```bash
git clone -b elk https://github.com/ruangsendiri/container-infra.git
```

## Usage

```bash
docker compose up -d

# show the kibana logs
docker logs kibana

# show the elasticsearch logs
docker logs elasticsearch

# show the logstash logs
docker logs logstash

# check elasticsearch health
curl -i -X GET "http://127.0.0.1:9200/_cluster/health?pretty"
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
