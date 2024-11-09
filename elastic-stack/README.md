- Install [mkcert](https://github.com/FiloSottile/mkcert)

- Ensure the environment variable `CAROOT` for the dev certificate CA is set

- Create the following dev certificates
  - ./certs/elastic.pem
  - ./certs/elastic-key.pem

- Run `docker compose up -d --build`
- Run `docker compose run --rm setup`