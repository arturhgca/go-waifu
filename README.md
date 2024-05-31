# go-waifu

## API spec

POST /requests
-> 202 returns a transaction ID

GET /requests/{transactionId}/status
-> 404 if missing
-> 200 with body explaining status

GET /requests/{transactionId}/output
-> 404 if missing
-> 200 with image

DELETE /requests/{transactionId}
-> 404 if missing
-> 204 if successful
