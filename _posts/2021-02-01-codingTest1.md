---
title: "프로그래머스 코딩 테스트 #1 K번째수"
categories:
  - React
tags:
  - Programmers
  - Coding Test
  - Javascript
  - Study
---

프로그래머스 사이트의 코딩테스트 연습   
[정렬 - K번째수](https://programmers.co.kr/learn/courses/30/lessons/42748)

```
function solution(array, commands) {
    var answer = [];
    commands.forEach(function(element){
        answer.push(array.slice(element[0] - 1, element[1]).sort((a,b)=> a-b)[element[2] - 1]);
    });   
    return answer;
}

solution([1, 5, 2, 6, 3, 7, 4], [[2, 5, 3], [4, 4, 1], [1, 7, 3]]);
```