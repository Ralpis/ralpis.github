### 기본연산

union #합집합

setdiff  #차집합

intersect #교집합

matrix(c(1,2,3,4),nrow=2) #행렬

matrix(c(1,2,3,4),nrow=2, byrow=T) #행을 기준으로

### 데이터프레임

표 형태로 쓰기 편하게끔 되어있는 자료형태

파이썬의 판다스 라이브러리도 R의 데이터프레임을 본따 만든 것 

data.frame(벡터값들) #데이터프레임 생성법

View(데이터프레임) #데이터프레임 출력



example[ ,2] #2번째 열을 보겠다

example$Price #원하는 컬럼을 뺄 수 있다



example[1, ] #1번째 행을 보겠다 데이터프레임형태로 반환을 한다

example[c(1,2), ] #1번째행과 2번째 행을 동시에 보는 법



### 특정조건에 맞는 행 추출

subset(원본데이터, 조건)

#특정 컬럼만 조회하고 싶을 때

subset(example, price >=100, select = name)

subset(example, price >=100, select = -price) #price빼고 

subset(example, price >=100, select = c(name,price))



### 외부데이터 불러오기

install.packages("readxl")

library(readxl)

외부데이터<- read_excel("example.xlsx")

외부데이터csv <-read.csv("example.csv")

외부데이터csv <-read.csv("example.csv",stringsAsFactors = F) #문자가 들어와있을 때,



### 데이터 저장하기

write.csv(example, file="example.csv")

save(example,file="example.rda")

load("example.rda") #데이터 불러오기

