# MyAppBar

## Links

| Title | Type | To or Action |
| :--- | :--- | :--- |
| Portafoglio | a | / |
| Menu \(Icon\) | popup |  |
| About | a | /about |
| New | a | /new |
| Random | a | /random |
| Avatar \(Icon\) | a | /users/:username/detail |
| Sign in | a | /signin |
| Sign out | a | call sign out function |

### Menu \(Icon\)

* 表示条件：有り\(Image参照\)
* popupメニューとし、内容はAbout、New、Randomへのリンクとする。

### New

* SiteList Component order="new"

### Random

* SiteList Component order="random"

### Avatar \(Icon\)

* 遷移条件：Sign in状態であること。Sign out状態の場合、/signinへリダイレクトする。

### Sign in

* 表示条件：Sign out状態であること。
* FirebaseUIを表示する

### Sign out

* 表示条件：Sign in状態であること。

## Required states

| Key | Remarks |
| :--- | :--- |
| user |  |





