# API v2

{% api-method method="get" host="" path="/v1/sites/" %}
{% api-method-summary %}
Get site list
{% endapi-method-summary %}

{% api-method-description %}
サイトのリストを取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="order" type="string" %}

{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "list": [
    {"name" "site name1", "comment1": "site comment1", "id": 1},
    {"name" "site name2", "comment2": "site comment2", "id": 2}
  ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/units/" %}
{% api-method-summary %}
Get units
{% endapi-method-summary %}

{% api-method-description %}
単位を取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "periodUnits": [
    { "value": "hour",  "label": "hour"  },
    { "value": "day",   "label": "day"   },
    { "value": "week",  "label": "week"  },
    { "value": "month", "label": "month" },
    { "value": "year",  "label": "year"  }
  ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/skills/" %}
{% api-method-summary %}
Get skills
{% endapi-method-summary %}

{% api-method-description %}
スキルを取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "skills": [
    { "value": "ruby",  "label": "ruby"  },
    { "value": "rails", "label": "rails" },
    { "value": "react", "label": "react" }
  ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/sites/:site\_id/reactions" %}
{% api-method-summary %}
Get reaction count of site
{% endapi-method-summary %}

{% api-method-description %}
サイトのリアクション数を取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="site\_id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "reactions": {
    "good": 1,
    "cool": 2
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/sites/:site\_id/views" %}
{% api-method-summary %}
Get view count of site
{% endapi-method-summary %}

{% api-method-description %}
サイトの閲覧数を取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="site\_id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "view": 1234
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/sites/:site\_id/info" %}
{% api-method-summary %}
Get site info
{% endapi-method-summary %}

{% api-method-description %}
サイトの情報を取得する。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="site\_id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "siteInfo": {
    "owner":      "john smith",
    "siteName":   "portafoglio",
    "siteUrl" :   "http://www.example.com",
    "period":     1,
    "periodUnit": "day",
    "usedSkills": [
                    { "value": "ruby",  "label": "ruby"  },
                    { "value": "rails", "label": "rails" },
                    { "value": "react", "label": "react" }
    ],
    "comment":    "something comment",
    "updateAt":   "2019/04/30"
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/sites/:site\_id/auth" %}
{% api-method-summary %}
Get site owner authentication
{% endapi-method-summary %}

{% api-method-description %}
　サイト所有者の認証をする。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="site\_id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-form-data-parameters %}
{% api-method-parameter name="token" type="string" required=true %}
　メールアドレス
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success",
  "result": "true" or "false"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="" path="/v1/sites/:site\_id/info" %}
{% api-method-summary %}
Post site info
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="site\_id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Firebase id token
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-form-data-parameters %}
{% api-method-parameter name="comment" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="usedSkills" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="periodUnit" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="period" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="siteUrl" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="siteName" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "message": "Success"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

