php74 + mailhog

もしもmailhogのログがウザければ消すDockerfileを作る

```
FROM mailhog/mailhog:latest

ENTRYPOINT ["/bin/sh", "-c", "MailHog &>/dev/null"]
```
