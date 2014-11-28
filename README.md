For more details about this cartridge please visit:
 
REPO-CONNECTOR
==========================================================

# Technical stuff

## Header

```
application/vnd.uptodator.repo-connector.v1+json
```
 
## HTTP Method:

```
GET 
```

## URL

```
/dependency/status
```

## BODY

I will receive

```
{
    "dependencies": [
        "com.ofg:micro-infra-spring:0.7.1",
        "com.ofg:micro-deps:0.5.2"
    ]
}
```

I will reply with

```
{
    "dependencies": {
        "com.ofg:micro-infra-spring": {
            "status" : "old",
            "newversion" : "0.8.1"
        },
        "com.ofg:micro-deps": {
            "status" : "uptodate"
        }
    }
}
```

# OPENSHIFT STUFF

https://github.com/vert-x/openshift-cartridge
