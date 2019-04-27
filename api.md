# API

POSTは作成、PATCHは部分更新、PUTは置換

```text
BASE /api/v1
```

| Method | URL | Receiv Params |
| :--- | :--- | :--- |
| POST | /signin | pending... |
| DELETE | /signout |  |
| GET | /sites/:site\_id |  |
| GET | /sites |  |
| GET | /sites/new |  |
| GET | /sites/random |  |
| PUT | /users/:username/avatar | avatar data \(DATA URI\) |
| DELETE | /users/:username/avatar |  |
| GET | /users/:username/skills |  |
| PATCH | /users/:username/skill | name, level |
| DELETE | /users/:username |  |
| PUT | /users/:username/detail | nickname, username, email, skills, sns ids |
| PUT | /sites/:site\_id/screenshot |  |
| DELETE | /sites/:site\_id/screenshot |  |
| POST | /sites/:site\_id/reactions/:id |  |
| DELETE | /sites/:site\_id/reactions/:reaction\_id |  |
| POST | /sites/:site\_id/views |  |
| DELETE | /sites/:site\_id |  |



