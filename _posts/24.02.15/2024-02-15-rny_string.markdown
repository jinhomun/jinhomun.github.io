---
layout: post
title: "프로그래머스 기초트레이닝 Day18-5"
date: 2024-02-15 14:00:00 +0900
categories: Javascript
---

### rny_string😀

'm'과 "rn"이 모양이 비슷하게 생긴 점을 활용해 문자열에 장난을 하려고 합니다.<br> 문자열 rny_string이 주어질 때, rny_string의 모든 'm'을 "rn"으로 바꾼 문자열을 return 하는 solution 함수를 작성해 주세요.<br>

※ 제한 사항<br>
1 ≤ rny_string의 길이 ≤ 100<br>
rny_string은 영소문자로만 이루어져 있습니다.<br>

입출력 <br>

|rny_string|  result   |
| :-------: | :-------: |
| "masterpiece"| "rnasterpiece" |
|  "programmers" |"prograrnrners"  |
|  "jerry" |	"jerry"|
|  "burn" |"burn" |

<br>

```javascript
function solution(rny_string) {
    let str = '';
    for(let i in rny_string){
        str += (rny_string[i] === 'm' ? 'rn' : rny_string[i]);
    } 
    return str;
}
```
