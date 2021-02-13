# Spring data JPA Mongodb expressions

Parses (subset of) mongodb expressions and convert it to Specifications to be used to Spring-data-jpa project. 

## Examples:

```
{
  "lastName": "ibrahim",
  "$and": [
    {
      "birthDate": {"$gt": "1981-01-01"}
    },
    {
      "birthDate": {"$lte": "1985-10-10"}
    }
  ]
}
```

result:
`where last_name=? and birth_date>? and birth_date<=?`


## Thanks:
Special thanks for [Rashad Saif](https://github.com/rashadsaif) and Hamada alnoby for helping 
in the design and doing review for the code.  