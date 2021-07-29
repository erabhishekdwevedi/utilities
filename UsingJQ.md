# JQ 
jq is like sed for JSON data - you can use it to slice and filter and map and transform structured data with the same ease that sed, awk, grep and friends let you play with text.

jq is basically a utility to parse json from bash response.

#### Install JQ 
```
yum -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
yum -y install jq
````

#### Using JQ

Sample JSON

```

{
    "name": "Simple JQ Tutorial",
    "date": "29 July 2021",
    "objectives": {
      "objective": [
        {
          "topic": "Introduction",
          "description": "Introduction to JQ",
          "type": "Text"
        },
        {
          "topic": "Installation",
          "description": "Installation of JQ",
          "type": "Bash Commands"
        },
        {
          "topic": "Usage",
          "description": "Examples showing usage of JQ",
          "type": "Code"
        },
        {
          "topic": "Reference",
          "description": "References and Links",
          "type": "Hyperlinks"
        }
      ]
    }
  }

```

JQ can be used independently or used with response of other commands using pipe.

Prettify JSON 
```
jq "." sample.json
```

Pretty json response 

```
cat sample.json | jq "."
```


Getting name 
```
cat sample.json| jq -r ".name"
```

Response:
```
Simple JQ Tutorial
```

Get Description
```
cat sample.json| jq -r ".objectives.objective[0].description"
```
Response:
```
Introduction to JQ
```


Get All Objectives
```
cat sample.json| jq -r ".objectives.objective"
```
Response:
```
[
  {
    "topic": "Introduction",
    "description": "Introduction to JQ",
    "type": "Text"
  },
  {
    "topic": "Installation",
    "description": "Installation of JQ",
    "type": "Bash Commands"
  },
  {
    "topic": "Usage",
    "description": "Examples showing usage of JQ",
    "type": "Code"
  },
  {
    "topic": "Reference",
    "description": "References and Links",
    "type": "Hyperlinks"
  }
]

```
Slicing Array

```
jq ".objectives.objective[2,3]" sample.json
```

Response
```
{
  "topic": "Usage",
  "description": "Examples showing usage of JQ",
  "type": "Code"
}
{
  "topic": "Reference",
  "description": "References and Links",
  "type": "Hyperlinks"
}
```

#### Getting Keys From JSON Array

```
jq ".objectives.objective | keys" sample.json
````

RESPONSE

```
[
  0,
  1,
  2,
  3
]
```


#### Reference
* https://stedolan.github.io/jq/
















