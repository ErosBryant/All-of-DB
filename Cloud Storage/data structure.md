# Data 구조

#####  비관계형 데이터는 일반적으로 ***반구조적***과 ***비구조적***이라는 두 가지 범주로 구분됩니다. 
##### 비관계형 데이터는 테이블 집합으로 구조화되지 않은 모든 데이터를 의미하는 포괄적 용어입니다

##  반구조적 데이터
- 반구조적 데이터는 필드를 포함하는 데이터
- 데이터의 형식은 애플리케이션에서 구문을 분석하고 처리할 수 있는 방식
  - 일반적인 방법 중 하나는 JSON 
  - JavaScript Object Notation
  - JSON 문서는 중괄호({ 및 })
  -  배열로 유지되고 대괄호([ 및 ])

```java
            {
            "ID": "1",
            "Name": "Mark Hanson",
            "Telephone": [ 
                { "Home": "1-999-9999999" }, 
                { "Business": "1-888-8888888" }, 
                { "Cell": "1-777-7777777" }
            ],
            "Address": [ 
                { "Home": [
                { "StreetAddress": "121 Main Street" }, 
                { "City": "Some City" },
                { "State": "NY" }, 
                { "Zip": "10110" }
                ] },
                { "Business": [
                { "StreetAddress": "87 Big Building" },
                { "City": "Some City" },
                { "State": "NY" },
                { "Zip": "10111" }
                ] }
            ] 
            }
```
- 밖의 형식으로는 Avro, ORC, Parquet

## 비구조적 데이터
- 비구조적 데이터란 필드를 당연히 포함하지 않는 데이터입니다. 그 예로는 비디오, 오디오 및 기타 미디어 스트림이 있습니다. 각 항목은 비정형적 이진 데이터 blob입니다. 이 데이터의 특정 요소는 검색할 수 없습니다.

![image](https://user-images.githubusercontent.com/86946575/169189608-1ad779d4-b646-4bff-b829-53848fe40fe8.png)
