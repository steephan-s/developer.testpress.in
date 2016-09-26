# Mentors
Admin Mentors API gives you access to add/remove students to a mentor.

## View all mentors

```shell
curl --request GET \
  --url http://demo.testpress.in/api/v2.2/admin/mentors/ \
  --header 'authorization: JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs' \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/json' \
  --header 'postman-token: 05f143f7-6f58-1016-7fce-ac1c8389c22d'
```

```ruby
require 'uri'
require 'net/http'

url = URI("http://demo.testpress.in/api/v2.2/admin/mentors/")

http = Net::HTTP.new(url.host, url.port)

request = Net::HTTP::Get.new(url)
request["authorization"] = 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
request["content-type"] = 'application/json'
request["cache-control"] = 'no-cache'
request["postman-token"] = 'cf67008b-3e21-c9f7-239d-e7af76e7a482'

response = http.request(request)
puts response.read_body
```

```python
import requests

url = "http://demo.testpress.in/api/v2.2/admin/mentors/"

headers = {
    'authorization': "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    'content-type': "application/json",
    'cache-control': "no-cache",
    'postman-token': "8764dd74-c291-5fa5-a2c9-51ce8456bfaa"
    }

response = requests.request("GET", url, headers=headers)

print(response.text)
```

```csharp
var client = new RestClient("http://demo.testpress.in/api/v2.2/admin/mentors/");
var request = new RestRequest(Method.GET);
request.AddHeader("postman-token", "5f78f97b-86d4-0cd3-f34e-12ec5f89c409");
request.AddHeader("cache-control", "no-cache");
request.AddHeader("content-type", "application/json");
request.AddHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs");
IRestResponse response = client.Execute(request);
```

```php
<?php

$request = new HttpRequest();
$request->setUrl('http://demo.testpress.in/api/v2.2/admin/mentors/');
$request->setMethod(HTTP_METH_GET);

$request->setHeaders(array(
  'postman-token' => '1fb985fb-3d05-df98-8162-db765a59ca72',
  'cache-control' => 'no-cache',
  'content-type' => 'application/json',
  'authorization' => 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
));

try {
  $response = $request->send();

  echo $response->getBody();
} catch (HttpException $ex) {
  echo $ex;
}
```

```java
OkHttpClient client = new OkHttpClient();

Request request = new Request.Builder()
  .url("http://demo.testpress.in/api/v2.2/admin/mentors/")
  .get()
  .addHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
  .addHeader("content-type", "application/json")
  .addHeader("cache-control", "no-cache")
  .addHeader("postman-token", "5ac4e072-1f54-008f-9ddb-6225c57c3014")
  .build();

Response response = client.newCall(request).execute();
```

```javascript
var http = require("http");

var options = {
  "method": "GET",
  "hostname": "demo.testpress.in",
  "port": null,
  "path": "/api/v2.2/admin/mentors/",
  "headers": {
    "authorization": "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    "content-type": "application/json",
    "cache-control": "no-cache",
    "postman-token": "c0451db9-2ced-f0ca-66bc-05d63081f398"
  }
};

var req = http.request(options, function (res) {
  var chunks = [];

  res.on("data", function (chunk) {
    chunks.push(chunk);
  });

  res.on("end", function () {
    var body = Buffer.concat(chunks);
    console.log(body.toString());
  });
});

req.end();
```

```go
package main

import (
	"fmt"
	"net/http"
	"io/ioutil"
)

func main() {

	url := "http://demo.testpress.in/api/v2.2/admin/mentors/"

	req, _ := http.NewRequest("GET", url, nil)

	req.Header.Add("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
	req.Header.Add("content-type", "application/json")
	req.Header.Add("cache-control", "no-cache")
	req.Header.Add("postman-token", "49744256-fb7c-64c8-08a9-9832ff8f8b74")

	res, _ := http.DefaultClient.Do(req)

	defer res.Body.Close()
	body, _ := ioutil.ReadAll(res.Body)

	fmt.Println(res)
	fmt.Println(string(body))

}
```

> The above command returns JSON structured like this:

```json
[
    {
      "id": 2,
      "url": "http://demo.testpress.in/api/v2.2/admin/mentors/2/",
      "created": "2016-09-20T13:32:54.271Z",
      "user": 563,
      "students": [
        {
          "id": 2,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/2/",
          "first_name": "John",
          "last_name": "Appleseed",
          "email": "selvasteephandfasdfasdf@gmail.com",
          "gender": "Male"
        },
        {
          "id": 345,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/345/",
          "first_name": "hellouser",
          "last_name": "",
          "email": "testingsocialauth@gmail.com",
          "gender": null
        }
      ]
    },
    {
      "id": 1,
      "url": "http://demo.testpress.in/api/v2.2/admin/mentors/1/",
      "created": "2016-09-13T04:27:38.716Z",
      "user": 529,
      "students": [
        {
          "id": 345,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/345/",
          "first_name": "hellouser",
          "last_name": "",
          "email": "testingsocialauth@gmail.com",
          "gender": null
        },
        {
          "id": 2,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/2/",
          "first_name": "John",
          "last_name": "Appleseed",
          "email": "selvasteephandfasdfasdf@gmail.com",
          "gender": "Male"
        }
      ]
    },
    {
      "id": 16,
      "url": "http://demo.testpress.in/api/v2.2/admin/mentors/16/",
      "created": "2016-09-22T13:38:27.765Z",
      "user": 568,
      "students": [
        {
          "id": 2,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/2/",
          "first_name": "John",
          "last_name": "Appleseed",
          "email": "selvasteephandfasdfasdf@gmail.com",
          "gender": "Male"
        }
      ]
    }
  ]
```

This endpoint allows you to view all the mentors.

### HTTP Request

`GET /api/v2.2/admin/mentors/`

### Fields

Name | Type | Description
-----|------|-------------
id   | int  | The mentor unique ID
url  | string | URL to get details of the mentor
created | datetimefield | Date and time when mentor created
students | string | Pass as array of student details.


## View a mentor

```shell
curl --request GET \
  --url http://demo.testpress.in/api/v2.2/admin/mentors/2/ \
  --header 'authorization: JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs' \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/json' \
  --header 'postman-token: 99cc7320-a66f-6e44-301d-a008c6d43a4b'
```

```ruby
require 'uri'
require 'net/http'

url = URI("http://demo.testpress.in/api/v2.2/admin/mentors/2/")

http = Net::HTTP.new(url.host, url.port)

request = Net::HTTP::Get.new(url)
request["authorization"] = 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
request["content-type"] = 'application/json'
request["cache-control"] = 'no-cache'
request["postman-token"] = 'a5b42a83-06b0-9a4f-e932-47ac54f3140a'

response = http.request(request)
puts response.read_body
```

```python
import requests

url = "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

headers = {
    'authorization': "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    'content-type': "application/json",
    'cache-control': "no-cache",
    'postman-token': "079a621f-a2c9-76d5-b4c4-6b34c7edf9b7"
    }

response = requests.request("GET", url, headers=headers)

print(response.text)
```

```csharp
var client = new RestClient("http://demo.testpress.in:8000/api/v2.2/admin/mentors/2/");
var request = new RestRequest(Method.GET);
request.AddHeader("postman-token", "f841f54d-ee2c-d051-0aae-3787d163d30b");
request.AddHeader("cache-control", "no-cache");
request.AddHeader("content-type", "application/json");
request.AddHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs");
IRestResponse response = client.Execute(request);
```

```php
<?php

$request = new HttpRequest();
$request->setUrl('http://demo.testpress.in/api/v2.2/admin/mentors/2/');
$request->setMethod(HTTP_METH_GET);

$request->setHeaders(array(
  'postman-token' => 'f930f0a0-fd4f-7931-a27b-a0bdbf96cec4',
  'cache-control' => 'no-cache',
  'content-type' => 'application/json',
  'authorization' => 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
));

try {
  $response = $request->send();

  echo $response->getBody();
} catch (HttpException $ex) {
  echo $ex;
}
```

```java
OkHttpClient client = new OkHttpClient();

Request request = new Request.Builder()
  .url("http://demo.testpress.in/api/v2.2/admin/mentors/2/")
  .get()
  .addHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
  .addHeader("content-type", "application/json")
  .addHeader("cache-control", "no-cache")
  .addHeader("postman-token", "10829a19-b4c0-398d-cad4-3b7c99cc5693")
  .build();

Response response = client.newCall(request).execute();
```

```javascript
var http = require("http");

var options = {
  "method": "GET",
  "hostname": "demo.testpress.in",
  "port": null,
  "path": "/api/v2.2/admin/mentors/2/",
  "headers": {
    "authorization": "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    "content-type": "application/json",
    "cache-control": "no-cache",
    "postman-token": "858faeea-7788-8952-9755-8042876bb8a1"
  }
};

var req = http.request(options, function (res) {
  var chunks = [];

  res.on("data", function (chunk) {
    chunks.push(chunk);
  });

  res.on("end", function () {
    var body = Buffer.concat(chunks);
    console.log(body.toString());
  });
});

req.end();
```

```go
package main

import (
	"fmt"
	"net/http"
	"io/ioutil"
)

func main() {

	url := "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

	req, _ := http.NewRequest("GET", url, nil)

	req.Header.Add("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
	req.Header.Add("content-type", "application/json")
	req.Header.Add("cache-control", "no-cache")
	req.Header.Add("postman-token", "3ae80d6e-27a1-a1df-cd23-095c1148c83d")

	res, _ := http.DefaultClient.Do(req)

	defer res.Body.Close()
	body, _ := ioutil.ReadAll(res.Body)

	fmt.Println(res)
	fmt.Println(string(body))

}
```

```json
[
    {
      "id": 2,
      "url": "http://demo.testpress.in/api/v2.2/admin/mentors/2/",
      "students": [
        {
          "id": 2,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/2/",
          "username": "testpress",
          "first_name": "John",
          "last_name": "Appleseed",
          "display_name": "John Appleseed",
          "email": "selvasteephandfasdfasdf@gmail.com",
          "photo": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/d1b9192ef434443a963eced9b8747862.jpeg",
          "large_image": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/2e6f0eb3bc9d467ab4254c094b47611e.jpeg",
          "medium_image": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/7552ce50dff6479ba172f1102c56e72d.jpeg",
          "small_image": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/05764a619f09474d93caf0d49a43a4c0.jpeg",
          "x_small_image": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/5ae9976cc2224e08ab81510404dd8c93.jpeg",
          "mini_image": "https://s3-ap-southeast-1.amazonaws.com/media.testpress.in/i/34d189e496f140b3aa772ee19df46e1b.jpeg",
          "birth_date": "27/08/1994",
          "gender_code": "male",
          "gender": "Male",
          "address1": "Chennai",
          "address2": "Chennai",
          "city": "Chennai",
          "zip": "600069",
          "state": "",
          "state_code": "",
          "phone": "9043570576",
          "batches": [
            {
              "id": 30,
              "name": "Testing Batch 1",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/30/"
            },
            {
              "id": 29,
              "name": "new sample batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/29/"
            },
            {
              "id": 28,
              "name": "9th Students Tambaram 2016",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/28/"
            },
            {
              "id": 27,
              "name": "8th Standard Tambaram 2016",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/27/"
            },
            {
              "id": 26,
              "name": "UPSC Evening Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/26/"
            },
            {
              "id": 25,
              "name": "IBPS Online Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/25/"
            },
            {
              "id": 24,
              "name": "NEET Morning Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/24/"
            },
            {
              "id": 23,
              "name": "UPSC Morning  Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/23/"
            },
            {
              "id": 22,
              "name": "IBPS Morning Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/22/"
            },
            {
              "id": 21,
              "name": "st std A",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/21/"
            },
            {
              "id": 20,
              "name": "OHC 2013",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/20/"
            },
            {
              "id": 19,
              "name": "POZITIVE ONLINE TEST SERIES",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/19/"
            },
            {
              "id": 18,
              "name": "Unique UPSC Batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/18/"
            },
            {
              "id": 17,
              "name": "ECE",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/17/"
            },
            {
              "id": 16,
              "name": "EEE",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/16/"
            },
            {
              "id": 15,
              "name": "DISHA BATCH 1",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/15/"
            }
          ],
          "batches_url": "http://demo.testpress.in/api/v2.2/admin/users/2/batches/"
        },
        {
          "id": 345,
          "url": "http://demo.testpress.in/api/v2.2/admin/users/345/",
          "username": "hellouser",
          "first_name": "hellouser",
          "last_name": "",
          "display_name": "hellouser",
          "email": "testingsocialauth@gmail.com",
          "photo": null,
          "large_image": "",
          "medium_image": "",
          "small_image": "",
          "x_small_image": "",
          "mini_image": "",
          "birth_date": null,
          "gender_code": null,
          "gender": null,
          "address1": "",
          "address2": "",
          "city": "",
          "zip": "",
          "state": "",
          "state_code": "",
          "phone": "9898989898",
          "batches": [
            {
              "id": 29,
              "name": "new sample batch",
              "url": "http://demo.testpress.in/api/v2.2/admin/batches/29/"
            }
          ],
          "batches_url": "http://demo.testpress.in/api/v2.2/admin/users/345/batches/"
        }
      ]
    }
  ]
```

This endpoint allows you to view details of a particular mentor.

### HTTP Request

`GET /api/v2.2/admin/mentors/<:id>`

### URL Parameters

Parameter | Description
--------- | ------- | -----------
id | Unique Id of the mentor to retrieve

### Fields

Name | Type | Description
-----|------|-------------
id   | int  | The mentor unique ID
url  | string | URL to get details of the mentor
students | string | List of students belongs to the mentor

## Add a student

```shell
curl --request POST \
  --url http://demo.testpress.in/api/v2.2/admin/mentors/2/ \
  --header 'authorization: JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs' \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/x-www-form-urlencoded' \
  --header 'postman-token: be1c0d50-5586-16f5-5a50-a3b57243f23f' \
  --data student=payuser
```

```ruby
require 'uri'
require 'net/http'

url = URI("http://demo.testpress.in/api/v2.2/admin/mentors/2/")

http = Net::HTTP.new(url.host, url.port)

request = Net::HTTP::Post.new(url)
request["authorization"] = 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
request["content-type"] = 'application/x-www-form-urlencoded'
request["cache-control"] = 'no-cache'
request["postman-token"] = 'ad5e5f07-3380-fffa-aab5-c059cd263616'
request.body = "student=payuser"

response = http.request(request)
puts response.read_body
```

```python
import requests

url = "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

payload = "student=payuser"
headers = {
    'authorization': "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    'content-type': "application/x-www-form-urlencoded",
    'cache-control': "no-cache",
    'postman-token': "158579e5-22c5-46e4-7cc8-6e61b964619a"
    }

response = requests.request("POST", url, data=payload, headers=headers)

print(response.text)
```

```csharp
var client = new RestClient("http://demo.testpress.in/api/v2.2/admin/mentors/2/");
var request = new RestRequest(Method.POST);
request.AddHeader("postman-token", "e3405e68-0108-820c-c1b4-b30584913a28");
request.AddHeader("cache-control", "no-cache");
request.AddHeader("content-type", "application/x-www-form-urlencoded");
request.AddHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs");
request.AddParameter("application/x-www-form-urlencoded", "student=payuser", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```php
<?php

$request = new HttpRequest();
$request->setUrl('http://demo.testpress.in/api/v2.2/admin/mentors/2/');
$request->setMethod(HTTP_METH_POST);

$request->setHeaders(array(
  'postman-token' => 'f35aef33-504e-2dbb-4727-f6a20540e3d5',
  'cache-control' => 'no-cache',
  'content-type' => 'application/x-www-form-urlencoded',
  'authorization' => 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
));

$request->setContentType('application/x-www-form-urlencoded');
$request->setPostFields(array(
  'student' => 'payuser'
));

try {
  $response = $request->send();

  echo $response->getBody();
} catch (HttpException $ex) {
  echo $ex;
}
```

```java
OkHttpClient client = new OkHttpClient();

MediaType mediaType = MediaType.parse("application/x-www-form-urlencoded");
RequestBody body = RequestBody.create(mediaType, "student=payuser");
Request request = new Request.Builder()
  .url("http://demo.testpress.in/api/v2.2/admin/mentors/2/")
  .post(body)
  .addHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
  .addHeader("content-type", "application/x-www-form-urlencoded")
  .addHeader("cache-control", "no-cache")
  .addHeader("postman-token", "2452a04d-2a24-da1a-7e33-c6a23a4ed5a2")
  .build();

Response response = client.newCall(request).execute();
```

```javascript
var qs = require("querystring");
var http = require("http");

var options = {
  "method": "POST",
  "hostname": "demo.testpress.in",
  "port": null,
  "path": "/api/v2.2/admin/mentors/2/",
  "headers": {
    "authorization": "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    "content-type": "application/x-www-form-urlencoded",
    "cache-control": "no-cache",
    "postman-token": "e38548f9-7b59-43ab-078d-090bcdb9ff61"
  }
};

var req = http.request(options, function (res) {
  var chunks = [];

  res.on("data", function (chunk) {
    chunks.push(chunk);
  });

  res.on("end", function () {
    var body = Buffer.concat(chunks);
    console.log(body.toString());
  });
});

req.write(qs.stringify({ student: 'payuser' }));
req.end();
```

```go
package main

import (
	"fmt"
	"strings"
	"net/http"
	"io/ioutil"
)

func main() {

	url := "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

	payload := strings.NewReader("student=payuser")

	req, _ := http.NewRequest("POST", url, payload)

	req.Header.Add("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
	req.Header.Add("content-type", "application/x-www-form-urlencoded")
	req.Header.Add("cache-control", "no-cache")
	req.Header.Add("postman-token", "499585d8-a8fb-1732-5054-26da964bcab2")

	res, _ := http.DefaultClient.Do(req)

	defer res.Body.Close()
	body, _ := ioutil.ReadAll(res.Body)

	fmt.Println(res)
	fmt.Println(string(body))

}
```

> The above command returns JSON structured like this:

```json
{
  "student": "payuser"
}
```
This endpoint allows you to add a student to mentor

### HTTP Request

`POST /api/v2.2/admin/mentors/<:id>`

### URL Parameters

Parameter | Description
--------- | ------- | -----------
id | Unique Id of the mentor to retrieve

### POST data

Parameter | Description
--------- | ------- | -----------
student | Username of a student

### Response Fields

Name | Type | Description
-----|------|-------------
student | string | Username of the student

## Remove a student

```shell
curl --request DELETE \
  --url http://demo.testpress.in/api/v2.2/admin/mentors/2/ \
  --header 'authorization: JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs' \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/x-www-form-urlencoded' \
  --header 'postman-token: a25a8044-225b-50b2-74d9-dee498c1e7a5' \
  --data student=payuser
```

```ruby
require 'uri'
require 'net/http'

url = URI("http://demo.testpress.in/api/v2.2/admin/mentors/2/")

http = Net::HTTP.new(url.host, url.port)

request = Net::HTTP::Delete.new(url)
request["authorization"] = 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
request["content-type"] = 'application/x-www-form-urlencoded'
request["cache-control"] = 'no-cache'
request["postman-token"] = '667a6898-9b2a-600b-da23-a08b0970db5e'
request.body = "student=payuser"

response = http.request(request)
puts response.read_body
```

```python
import requests

url = "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

payload = "student=payuser"
headers = {
    'authorization': "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    'content-type': "application/x-www-form-urlencoded",
    'cache-control': "no-cache",
    'postman-token': "35783d6c-740a-6d4a-f777-79573c5778e6"
    }

response = requests.request("DELETE", url, data=payload, headers=headers)

print(response.text)
```

```csharp
var client = new RestClient("http://demo.testpress.in/api/v2.2/admin/mentors/2/");
var request = new RestRequest(Method.DELETE);
request.AddHeader("postman-token", "1ecdc349-aa3d-7a00-8551-55b078721492");
request.AddHeader("cache-control", "no-cache");
request.AddHeader("content-type", "application/x-www-form-urlencoded");
request.AddHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs");
request.AddParameter("application/x-www-form-urlencoded", "student=payuser", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```php
<?php

$request = new HttpRequest();
$request->setUrl('http://demo.testpress.in/api/v2.2/admin/mentors/2/');
$request->setMethod(HTTP_METH_DELETE);

$request->setHeaders(array(
  'postman-token' => 'a1e53319-7107-d2fc-707d-4f75999eaee6',
  'cache-control' => 'no-cache',
  'content-type' => 'application/x-www-form-urlencoded',
  'authorization' => 'JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs'
));

$request->setContentType('application/x-www-form-urlencoded');
$request->setPostFields(array(
  'student' => 'payuser'
));

try {
  $response = $request->send();

  echo $response->getBody();
} catch (HttpException $ex) {
  echo $ex;
}
```

```java
OkHttpClient client = new OkHttpClient();

MediaType mediaType = MediaType.parse("application/x-www-form-urlencoded");
RequestBody body = RequestBody.create(mediaType, "student=payuser");
Request request = new Request.Builder()
  .url("http://demo.testpress.in/api/v2.2/admin/mentors/2/")
  .delete(body)
  .addHeader("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
  .addHeader("content-type", "application/x-www-form-urlencoded")
  .addHeader("cache-control", "no-cache")
  .addHeader("postman-token", "e3b7aa4e-5940-eff2-6e56-dcdc713d10b8")
  .build();

Response response = client.newCall(request).execute();
```

```javascript
var qs = require("querystring");
var http = require("http");

var options = {
  "method": "DELETE",
  "hostname": "demo.testpress.in",
  "port": null,
  "path": "/api/v2.2/admin/mentors/2/",
  "headers": {
    "authorization": "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs",
    "content-type": "application/x-www-form-urlencoded",
    "cache-control": "no-cache",
    "postman-token": "5a272546-d7c8-76aa-27c2-26a4d94298fe"
  }
};

var req = http.request(options, function (res) {
  var chunks = [];

  res.on("data", function (chunk) {
    chunks.push(chunk);
  });

  res.on("end", function () {
    var body = Buffer.concat(chunks);
    console.log(body.toString());
  });
});

req.write(qs.stringify({ student: 'payuser' }));
req.end();
```

```go
package main

import (
	"fmt"
	"strings"
	"net/http"
	"io/ioutil"
)

func main() {

	url := "http://demo.testpress.in/api/v2.2/admin/mentors/2/"

	payload := strings.NewReader("student=payuser")

	req, _ := http.NewRequest("DELETE", url, payload)

	req.Header.Add("authorization", "JWT eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6MzgsInVzZXJfaWQiOjM4LCJlbWFpbCI6InN0ZWVwaGFuc2VsdmFyYWpAdGVzdHByZXNzLmluIiwiZXhwIjoxNDc0ODc3MjQwfQ.qXR2rR624oZztgH6GKbI9LY_MGBsKqUikM4JBNgeujs")
	req.Header.Add("content-type", "application/x-www-form-urlencoded")
	req.Header.Add("cache-control", "no-cache")
	req.Header.Add("postman-token", "8e9714b4-4093-b9dd-2c6a-46216bffb059")

	res, _ := http.DefaultClient.Do(req)

	defer res.Body.Close()
	body, _ := ioutil.ReadAll(res.Body)

	fmt.Println(res)
	fmt.Println(string(body))

}
```
> The above command on success will return 204 NO CONTENT

This endpoint allows you to remove a student from mentor

### HTTP Request

`DELETE /api/v2.2/admin/mentors/<:id>`

### URL Parameters

Parameter | Description
--------- | ------- | -----------
id | Unique Id of the mentor to retrieve

### POST data

Parameter | Description
--------- | ------- | -----------
student | Username of a student

