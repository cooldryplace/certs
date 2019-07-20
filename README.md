# Self signed certificates for gRPC

## Tools
CFSSL: Cloudflare's PKI and TLS toolkit https://cfssl.org

`go get -u github.com/cloudflare/cfssl/cmd/cfssl`
`go get -u github.com/cloudflare/cfssl/cmd/cfssljson`

## Generation

### CA
`cfssl gencert -initca ca-csr.json | cfssljson -bare ca`
