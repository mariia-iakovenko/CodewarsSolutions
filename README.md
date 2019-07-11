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
#### Sum of Digits / Digital Root 6kyu
*https://www.codewars.com/kata/sum-of-digits-slash-digital-root/train/javascript

```javascript
function digital_root(n) {
 if(n === 0){
     return 0;
   }else if(n > 9){
     return (n - 9*Math.floor((n-1)/9));
   }else if(n < 9){
     return n;
   }
}
```
#### Difference Of Squares 7kyu
*https://www.codewars.com/kata/difference-of-squares/train/javascript

```javascript
function differenceOfSquares(n){
let sum2 = 0;
  for(let i = 1; i <= n; i++){
  sum2 += i*i;
  }
let sum1 = 0;
  for(let i = 1; i <= n; i++){
  sum1 += i;
  }
return sum1*sum1 - sum2;
}
```
* new solution
----
****

#### Reversed Strings 8kyu
*https://www.codewars.com/kata/reversed-strings/train/javascript

```javascript
function solution(str){
  let str1 = '';
  for(let i = str.length - 1; i >= 0; i--){
  str1 += str[i];
  }
  return str1;
}
```

#### Calculate average 8kyu
*https://www.codewars.com/kata/calculate-average/train/javascript

```javascript
function find_average(arr) {
let sum = 0;
  for(let i = 0; i < arr.length; i++){
  sum += arr[i];
  }
  return sum / arr.length;
}
```
#### Reserved String 8kyu
```javascript
function solution(str){
  return str.split('').reverse().join('');  
}
```

#### Mumbling 7kyu
*https://www.codewars.com/kata/mumbling/train/javascript

```javascript
function accum(s) {
 let s1 = '';
  for(let i = 0; i < s.length; i++){
  s1 += s[i].toUpperCase() + s[i].toLowerCase().repeat(i) + '-';

  }
   return s1.slice(0, -1);
}
```
#### Reverse a Number 7kyu
*https://www.codewars.com/kata/555bfd6f9f9f52680f0000c5

```javascript
function reverseNumber(n) {
  if(n < 0){
  n = n * (-1);
  n = n.toString().split('').reverse().join('');
  n = +(n);
  return n * (-1);
  }
  if(n >= 0){return +(n.toString().split('').reverse().join(''));}
}
```
#### Simple beads count 7kyu
*https://www.codewars.com/kata/58712dfa5c538b6fc7000569

```javascript
function countRedBeads(n) {
if(n < 2){
return 0;
}else{
return n * 2 - 2;
}

}
```
#### Initialize my name 7kyu
*https://www.codewars.com/kata/initialize-my-name/train/javascript

```javascript
function initializeNames(name){
  let arr = name.split(' ');
  for(let i = 1; i < arr.length - 1; i++){
  arr[i] = arr[i].substring(0, 1) + '.';
  }
  let newName = arr.join(' ');
  return newName;
}
```
#### Array Array Array 7kyu
*https://www.codewars.com/kata/array-array-array/train/javascript

```javascript
function explode(x){
let arr = [];
  if(typeof x[0] === 'number'){ 
    for(let i = 1; i <= x[0]; i++){
    arr.push(x);
    }
  }
  
  if(typeof x[1] === 'number'){ 
  for(let i = 1; i <= x[1]; i++){
    arr.push(x);
    }
  }
if(typeof x[0] !== 'number'&& typeof x[1] !== 'number'){
return 'Void!'
}
return arr;
}
```
#### Create Four Letter Birding Codes from Bird Names 6kyu
*https://www.codewars.com/kata/create-four-letter-birding-codes-from-bird-names/train/javascript

```javascript
function birdCode(arr){
let newArr = [];
let bird = [];
  for(let i = 0; i < arr.length; i++){
  newArr.push(arr[i].split(/[^a-zA-Z,']+/g));
  }
 for (let i = 0; i < newArr.length; i++) {
  for (let j = 0; j < newArr[i].length; j++) {
    if (newArr[i].length === 1) {
      bird.push(newArr[i][j].substring(0, 4).toUpperCase());
    break;
    }
    if (newArr[i].length === 2) {
      bird.push((newArr[i][0].substring(0, 2) + newArr[i][1].substring(0, 2)).toUpperCase());
    break;
    }
    if (newArr[i].length === 3) {
      bird.push((newArr[i][0].substring(0, 1) + newArr[i][1].substring(0, 1) + newArr[i][2].substring(0, 2)).toUpperCase());
    break;
    }
    if (newArr[i].length === 4) {
      bird.push((newArr[i][0].substring(0, 1) + newArr[i][1].substring(0, 1) + newArr[i][2].substring(0, 1) + newArr[i][3].substring(0, 1)).toUpperCase());
    break;
    }
  }
}
  return bird;
}
```
#### Remove duplicates from list 8kyu

*https://www.codewars.com/kata/remove-duplicates-from-list/train/javascript

```javascript
function distinct(a) {
let uniqueNumbers = [];
    for(var i in a){
        if(uniqueNumbers.indexOf(a[i]) === -1){
            uniqueNumbers.push(a[i]);
        }
    }
    return uniqueNumbers;
}
```