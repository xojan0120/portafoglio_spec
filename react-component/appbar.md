---
description: 各ページ共通のナビゲーションバー
---

# MyAppBar

## Links

| Ttile | Type | To |
| :--- | :--- | :--- |
| Portafoglio | a | / |
| Menu \(Icon\) | popup |  |
| About | a | /about |
| New | a | /new |
| Random | a | /random |
| Avatar \(Icon\) | a | /profile |
| Sign in | a | /signin |
| Sign out | a | /signout |

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
* Firebase認証へのリンク
* リクエストtoAPI：signin

### Sign out

* 表示条件：Sign in状態であること。
* リクエストtoAPI：signout

## States to use

| Key | Type | Default value |
| :--- | :--- | :--- |
| login | boolean | false |

## Functions to use



