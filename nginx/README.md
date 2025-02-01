- Install [mkcert](https://github.com/FiloSottile/mkcert)

- Execute the following command: \
  ```
  mkcert -cert-file certs/cert.pem -key-file certs/cert-key.pem `
  apm.local `
  elasticsearch.local `
  kafka-ui.local `
  kafka.local `
  kibana.local `
  keycloak.local `
  pg-admin.local
  ```

  This will create the following dev certificates:
  - ./certs/cert.pem
  - ./certs/cert-key.pem

- Run `docker compose up -d`

- Add the configured services to the hosts file