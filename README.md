# Oracle SQL 공부한 것을 메모하는 공간입니다.
>2015-10-26

## DML (Data Manipulation Language)

### 1. INSERT : 삽입
`
INSERT INTO tableName (columnName ... ) VALUES (value ... )
` 
<br>
<br>
테이블에 저장할 값(value)은 해당 컬럼(columnName)과 데이터 타입이 일치하여야 한다. 

### 2. SELECT : 조회
`
SELECT * FROM tableName : 해당 테이블(tableName)의 모든 정보를 출력한다.
`
<br>
`
SELECT columnName ... FROM tableName : 해당 테이블(tableName)에서 선택한 정보(columnName)만 출력한다.
`

#### 
### 3. UPDATE : 수정
`
NUMBER(precision, scale)
`
### 4. DELETE : 삭제
`
NUMBER(precision, scale)
`

## Oracle 에서 자주 쓰이는 데이터 타입

##### 1. NUMBER : 숫자 데이터를 저장하기 위해서 제공됩니다.

`
NUMBER(precision, scale)
`
<br>
<br>
<b>precision</b>은 소수점을 포함한 전체자리수를 의미하며, <b>scale</b>은 소수점 이하 자리수를 지정합니다.<br>

##### 2. DATE : 세기, 년, 월, 일, 시간, 분, 초의 날짜 및 시간데이터를 저장하기 위해 제공됩니다.

`
DATE : 기본 날짜 형식은 "YY/MM/DD" 형식으로 "년/월/일" 로 출력된다.
`

##### 3. VARCHAR2 : 가변적인 길이의 문자열을 저장하기 위해서 제공합니다.
`
VARCHAR2(length) : length 보다 짧은 문자열을 입력한 경우, 저장 공간을 낭비하지 않는다.
`
<br>
`
CHAR(length) : 주어진 크기만큼 저장공간이 할당되므로, 저장공간의 낭비가 발생할 수 있다.
`



## 데이터의 구조를 살펴보기 위한 DESC

`
DESC tableName
`
<br>
<br>
<b> DESC 명령어는 컬럼 이름, 데이터 타입, 길이와 NULL 허용 유무 등과 같은 특정 테이블의 정보를 알려줍니다.</b>

## 테이블을 생성하는 CREATE TABLE

`
CREATE TABLE tableName (columnName1 columnType1, columnName2 columnType2, columnName3 columnType3 ...)
`

#### 식별자의 선언
컬럼명이나 테이블을 선언하기 위해서는 다음과 같은 원칙을 지켜야 합니다.

1. 시작은 반드시 영문자이어야 한다.
2. 예약어(SELECT 등)는 쓸 수 없다.
3. 유일한 단어이어야 한다.
4. _, $, #은 사용가능하다.

#### 컬럼 


>~ 2015-10-26 
