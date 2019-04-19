# API

POSTは作成、PATCHは部分更新、PUTは置換

```text
BASE /api/v1
```

| Method | URL | Receiv Params |
| :--- | :--- | :--- |
| POST | /signin | pending... |
| DELETE | /signout |  |
| GET | /portafoglios/:id |  |
| GET | /portafoglios |  |
| GET | /portafoglios/new |  |
| GET | /portafoglios/random |  |
| PUT | /users/:id/avatar | avatar data \(DATA URI\) |
| DELETE | /users/:id/avatar |  |
| GET | /users/:id/skills |  |
| PATCH | /users/:id/skill | name, level |
| DELETE | /users/:id |  |
| PUT | /users/:id/profile | nickname, username, email, skills, sns ids |
| PUT | /portafoglios/:id/screenshot |  |
| DELETE | /portafoglios/:id/screenshot |  |
| POST | /portafoglios/:site\_id/reactions/:reaction\_id |  |
| DELETE | /portafoglios/:site\_id/reactions/:reaction\_id |  |
| POST | /portafoglios/:id/views |  |



