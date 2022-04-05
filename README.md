# SpringBoot_REST_API
SpringBootでREST APIを作成する。

## 起動

``` bash
mvn clean spring-boot:run
```

## API呼び出し

### 引数なし

``` bash 
curl -s localhost:8080/greeting | jq
```

``` json 
{
  "id": 1,
  "content": "Hello, World!"
}
```

### 引数あり

``` bash
curl -s localhost:8080/greeting?user=hogehoge | jq   
```

``` json
{
  "id": 2,
  "content": "Hello, World!"
}
```

## 参考

- [Spring Boot REST API の作成](https://spring.pleiades.io/guides/gs/rest-service/)