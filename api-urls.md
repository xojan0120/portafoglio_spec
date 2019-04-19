# API

POSTは作成、PATCHは部分更新、PUTは置換

```text
BASE /api/v1
```

| Method | URL | Receiv Params |
| :--- | :--- | :--- |
| POST | /signin | pending... |
| DELETE | /signout |  |
| GET | /portafoglios/:site\_id |  |
| GET | /portafoglios |  |
| GET | /portafoglios/new |  |
| GET | /portafoglios/random |  |
| PUT | /users/:username/avatar | avatar data \(DATA URI\) |
| DELETE | /users/:username/avatar |  |
| GET | /users/:username/skills |  |
| PATCH | /users/:username/skill | name, level |
| DELETE | /users/:username |  |
| PUT | /users/:username/detail | nickname, username, email, skills, sns ids |
| PUT | /portafoglios/:site\_id/screenshot |  |
| DELETE | /portafoglios/:site\_id/screenshot |  |
| POST | /portafoglios/:site\_id/reactions/:id |  |
| DELETE | /portafoglios/:site\_id/reactions/:reaction\_id |  |
| POST | /portafoglios/:site\_id/views |  |
| DELETE | /portafoglios/:site\_id |  |



