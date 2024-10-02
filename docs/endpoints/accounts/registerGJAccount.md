# Register Account

> This endpoint is used to register an account
```
http://www.boomlings.com/database/accounts/registerGJAccount.php
```
> the https endpoint should also work
```
https://www.boomlings.com/database/accounts/registerGJAccount.php
```

## Parameters

| Parameter | Explanation | Optional |
| --- | --- | --- |
| `userName` | The username of the account to create | `False` |
| `gjp2` | The sha1 hash of the password , salt is: `mI29fmAnxgTs` | `True` (as long as no password param was given) |
| `password` | The password of the account to create | `False` |
| `email` | The email of the account to create | `False` |
| `secret` | Account Secret: `Wmfv3899gc9` | `False` |

## Response

**Successful Request**

```
1
```

**Failed Request**

| Error Code | Meaning |
| --- | --- |
| -1 | Generic Error |
| -2 | Username taken |
| -3 | Email taken |
| -4 | Username is longer than 20 characters |
| -5 | Invalid Password |
| -6 | Invalid Email / Ratelimited Registration (2 registrations per hour is the known ratelimit) |
| -8 | Password to short |
| -9 | Username to short |
