# Certbot

- [Certbot](https://certbot.eff.org/)

## Installation

Install with [Homebrew](Homebrew.md).

```bash
brew install certbot
sudo certbot certonly
```

## Usage

### Obtaining certificates

```bash
sudo certbot certonly --manual -d example.com,www.example.com
```

### Renewing certificates

```bash
certbot renew
```

### Uploading certificates

```bash
sudo aws iam Upload-server-certificate \
    --server-certificate-name example.com-2018-01-28 \
    --certificate-body file:////etc/letsencrypt/live/example.com/fullchain.pem \
    --private-key file:////etc/letsencrypt/live/example.com/privkey.pem \
    --path /cloudfront/example.com-2018-01-28/
```
