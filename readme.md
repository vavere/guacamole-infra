# Apache Guacamole ar Gitea kā IDP

Demo projekts izveido lokāli Apache Guacamole infrastruktūru kā lieototājus izmantojot VK Gitea

## Sagatavošanās

Pirms startēšanas jāizveido `.env` ar sekojošiem noslēpumiem:

```
OAUTH2_PROXY_CLIENT_ID=...id...
OAUTH2_PROXY_CLIENT_SECRET=...secret...
OAUTH2_PROXY_COOKIE_SECRET=...secret....
```

`CLIENT_ID` un `CLIENT_SECRET` iegūst reģīstrējot Gitea jaunu lietotni, kurā kā _redirect url_ jānorāda: _http://localhost:8080/oauth2/callback_

## Izmantošana

```
docker compose up -d
```