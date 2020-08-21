### Install
```npm install```


### Run offline

```sls offline``` then invoke the aws lambda function with:

1) use the endpoint url printed in the offline server output

2) Invoke function from local
```
sls invoke local -f function-name
```

3) Invoke lambda function using aws cli with custom base url
```
aws lambda invoke /dev/null \
  --endpoint-url http://localhost:3002 \
  --function-name hello
```