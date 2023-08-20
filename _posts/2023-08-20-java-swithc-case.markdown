---
layout: post
title:  "switch/case"
date:   2023-07-23
last_modified_at: 2018-09-20
categories: [Jekyll Paper]
tags: [Getting Start]
---
##Switch/case 문
switch/case 문은 if 문과 비슷하지만 좀 더 일정한 형식이 있는 조건·판단문이다. switch/case 문의 구조는 다음과 같다.
```
switch(입력변수) {
    case 입력값1: ...
         break;
    case 입력값2: ...
         break;
    ...
    default: ...
         break;
}
```
입력 변수의 값과 일치하는 case 입력값(입력값1, 입력값2, …)이 있다면 해당 case 문에 속한 문장들이 실행된다. case 하나마다 break가 같이 있게되는데 해당 case 문을 실행한 뒤 switch 문을 끝내기 위한 것이다. 만약 break 문이 끝나 있다면 그 다음의 case 문에 속한 문장이 곧바로 시작된다.

####예시(1)
---
```
public class Sample {
    public static void main(String[] args) {
        int month = 8;
        String monthString = "";
        switch (month) {  // 입력 변수의 자료형은 byte, short, char, int, enum, String만 가능하다.
            case 1:  monthString = "January";
                     break;
            case 2:  monthString = "February";
                     break;
            case 3:  monthString = "March";
                     break;
            case 4:  monthString = "April";
                     break;
            case 5:  monthString = "May";
                     break;
            case 6:  monthString = "June";
                     break;
            case 7:  monthString = "July";
                     break;
            case 8:  monthString = "August";
                     break;
            case 9:  monthString = "September";
                     break;
            case 10: monthString = "October";
                     break;
            case 11: monthString = "November";
                     break;
            case 12: monthString = "December";
                     break;
            default: monthString = "Invalid month";
                     break;
        }
        System.out.println(monthString);
    }
}
```


```
August
```
--- 
switch 문의 입력이 1이면 January라는 문자열이, 12면 December라는 문자열이 출력되는 예제이다. 이 예제는 month가 8로 고정되어 있기 때문에 August가 출력될 것이다. switch 문은 month의 값이 1이면 case 1: 문장이 실행되고 2이면 case 2: 문장이, 3이면 case 3: … 이런 식으로 수행된다. 만약 month에 1에서 12 사이의 숫자가 아닌 다른 값이 저장되어 있다면 default: 문장이 수행된다.

이와 같이 입력값이 정형화되어 있는 경우 if 문보다는 switch/case 문을 쓰는 것이 코드의 가독성이 좋다.

` ` switch/case 문은 if 문으로 변경이 가능하지만 if 문으로 작성된 모든 코드를 switch 문으로 변경할 수는 없다.