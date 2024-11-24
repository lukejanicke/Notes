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
sudo certbot certonly --manual -d lukejanicke.com,www.lukejanicke.com
```

### Renewing certificates

```bash
certbot renew
```

### Uploading certificates

```bash
sudo aws iam Upload-server-certificate \
    --server-certificate-name lukejanicke.com-2018-01-28 \
    --certificate-body file:////etc/letsencrypt/live/lukejanicke.com/fullchain.pem \
    --private-key file:////etc/letsencrypt/live/lukejanicke.com/privkey.pem \
    --path /cloudfront/lukejanicke.com-2018-01-28/
```
