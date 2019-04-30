# Untitled

{% api-method method="get" host="https://api.cakes.com" path="/v1/sites/" %}
{% api-method-summary %}
Get site list
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get site list.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Firebase id token.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="order" type="string" %}
取得順
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "status": 200,
  "message": "success",
  "data": [
    {"name" "site name1", "comment1": "site comment1", "id": 1},
    {"name" "site name2", "comment2": "site comment2", "id": 2}
  ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "status": 404,
    "message": "Record not found."
    "data": []
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



