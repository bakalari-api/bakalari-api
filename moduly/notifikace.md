# Notifikace
Zobrazí počet notifikací za určité časové období.

Je potřeba zaslat POST request na `https://www.example.com/if/2/overview/notifications`

Uživatel se nepřihlašuje klasicky jako u ostatních endpointů, ale pomocí [Basic Authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). Uživatelské jméno je `ANDR`, heslo je token, který je používán při přihlašování u ostatních endpointů.

Basic Authentication funguje tak, že se pošle header `Authorization` s hodnotou `Basic <b64>`, kde `<b64>` je string `<jmeno>:<heslo>` zakódovaný do base64.

Vstup i výstup je tentokrát v JSONu, ne v XML.

Vstup:

```json
{
    "MessageType": "Overview.Notifications.Req",
    "classificationFrom": "20180101",
    "classificationTo": "20190103",
    "homeworksFrom": "20180101",
    "homeworksTo": "20190103"
}
```

Výstup:
```json
{
    "ClassificationCount": 0,
    "HomeworksCount": 0,
    "KomensMessagesCount": 0,
    "MessageType": "Overview.Notifications.Resp"
}
```
