## what is this?
Elasticsearch samples.

## build & run docker container
```
$ docker-compose build
$ docker-compose up -d
```

## create sample index
```
$ curl -X PUT "localhost:9200/blog" -H 'Content-Type:application/json' -d @blog-mapping.json
```

## add sample document
```
$ curl -X POST "localhost:9200/blog/_doc" -H 'Content-Type:application/json' -d @testdata/blog01.json
```

