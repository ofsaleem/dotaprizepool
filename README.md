# dotaprizepool
Slack command to show the current prizepool for the Dota 2 International

This uses AWS Lambda with a Python 2.7 runtime as well as an API Gateway.

You will need a mapping template in the integration request for content type `application/x-www-form-urlencoded` that reads:

```javascript
{
  "body" : $input.json('$')
}
```
