# NATS

```bash

brew tap nats-io/nats-tools
brew install nats-io/nats-tools/nats
brew install nats-io/nats-tools/nsc

```

## Run

```bash
docker compose up -d

# grafana: http://localhost:3000 (user/pass = admin/admin)
# prometheus: http://localhost:9090

nats bench testsubject --pub 10 --sub 10 --msgs 10000 --size 512
```

## Tips

- `nats cheat` for cheat sheet
- [Video: Effective debugging using the NATS CLI](https://www.youtube.com/watch?v=pf8jSMMuPr4) (10 min)
- [Playlist: Rethinking connectivity](https://www.youtube.com/playlist?list=PLgqCaaYodvKY22TpvwlsalIArTmc56W9h)
- [nats docker image (docs)](https://github.com/docker-library/docs/tree/master/nats) (official)
