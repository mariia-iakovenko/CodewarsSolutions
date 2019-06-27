Hello


======
#### String ends with? 7kyu
* https://www.codewars.com/kata/51f2d1cafc9c0f745c00037d
```javascript
function solution(str, ending){
  return str.endsWith(ending);
}
```
#### Returning Strings 8kyu
* https://www.codewars.com/kata/55a70521798b14d4750000a4

```javascript 
function greet(name){
  return 'Hello, '+ name + ' how are you doing today?'
}
```

#### Kata Example Twist 8kyu
* https://www.codewars.com/kata/kata-example-twist/train/javascript

```javascript
var websites = [];
for(let i = 0; i < 1000; i++){
websites.push('codewars');
}
```

#### Invert values 8kyu
* https://www.codewars.com/kata/invert-values/train/javascript

```javascript
function invert(array) {
const invertArray = [];
  for(let i = 0; i < array.length; i++){
  invertArray.push(-array[i]);
  }
   return invertArray;
}
```
#### Century From Year 8kyu
* https://www.codewars.com/kata/century-from-year/train/javascript

```javascript
function century(year) {
  return Math.ceil(year/100);
}
```
#### Square(n) Sum 8kyu
* https://www.codewars.com/kata/square-n-sum/train/javascript

```javascript
function squareSum(numbers){
let sum = 0;
let sumTotal = 0;
  for(let i = 0; i < numbers.length; i++){
  sum = Math.pow(numbers[i], 2);
  sumTotal += sum;
  }
  return sumTotal;
}
```

#### Check the exam 8kyu
*https://www.codewars.com/kata/check-the-exam/train/javascript

```javascript
function checkExam(array1, array2) {
let totalScore = 0;
  for (let i = 0; i < array1.length; i++){
    if(array1[i] === array2[i]){
    totalScore += 4;
    }else if (array2[i] === ''){
    totalScore += 0;
    }else{
    totalScore -= 1;
    }
  }
  if(totalScore < 0){
  return 0;
  }else{
  return totalScore;
  }
}
```
