# API

POSTは作成、PATCHは部分更新、PUTは置換

```text
BASE /api/v1
```

| Method | URL | Receiv Params |
| :--- | :--- | :--- |
| POST | /api/v1/signin | pending... |
| DELETE | /api/v1/signout |  |
| GET | /api/v1/portafoglios/:id |  |
| GET | /api/v1/portafoglios |  |
| GET | /api/v1/portafoglios/new |  |
| GET | /api/v1/portafoglios/random |  |
| PUT | /api/v1/users/:id/avatar | avatar data \(DATA URI\) |
| DELETE | /api/v1/users/:id/avatar |  |
| GET | /api/v1/users/:id/skills |  |
| PATCH | /api/v1/users/:id/skill | name, level |
| DELETE | /api/v1/users/:id |  |
| PUT | /api/v1/users/:id/profile | nickname, username, email, skills, sns ids |
| PUT | /api/v1/portafoglios/:id/screenshot |  |
| DELETE | /api/v1/portafoglios/:id/screenshot |  |
| POST | /api/v1/portafoglios/:site\_id/reactions/:reaction\_id |  |
| DELETE | /api/v1/portafoglios/:site\_id/reactions/:reaction\_id |  |
| POST | /api/vi1/portafoglios/:id/views |  |



