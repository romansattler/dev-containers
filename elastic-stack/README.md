- Install [mkcert](https://github.com/FiloSottile/mkcert)

- Ensure the environment variable `CAROOT` for the dev certificate CA is set

- Execute the following command: \
  ```
  mkcert -cert-file certs/elastic.pem -key-file certs/elastic-key.pem `
  localhost `
  es
  ```

  This will create the following dev certificates:
  - ./certs/cert.pem
  - ./certs/cert-key.pem
- Create the following dev certificates
  - ./certs/elastic.pem
  - ./certs/elastic-key.pem

- Run `docker compose up -d --build`
- Run `docker compose run --rm setup`