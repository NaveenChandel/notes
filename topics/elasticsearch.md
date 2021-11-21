## Docker container
https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-docker.html 

## Queries

```sh
PUT surveys/

GET surveys/_search

GET surveys-test/_search

DELETE surveys/

create index
PUT /my-index-000001

GET /customer_perception_test/_search
{
  "size": 20,
  "query": {"match": {"answers.dataType" : "text"}}
}

GET /customer_perception_test/_count

GET /customer_perception_test/_search
{
  "query": {"match_all": {}}
}

DELETE /customer_perception_test/_doc/lOULPHwBgxM6hNrTn-l6

PUT customer_perception_test/_mapping
{
  "mappings": {
    "properties": {
      "response.answers.answer": {
        "type": "string",
        "ignore_malformed": true
      }
    }
  }
}

POST customer_perception_test/_doc/
{}

GET _search
{
  "query": {
    "match_all": {}
  }
}

GET /_search

POST customer_perception_test/_doc/
{}

GET _search
{
  "query": {
    "match_all": {}
  }
}

GET /_search

GET /![image](https://user-images.githubusercontent.com/65451453/142763804-a2921908-d465-4daa-af14-736e914fe090.png)

```
