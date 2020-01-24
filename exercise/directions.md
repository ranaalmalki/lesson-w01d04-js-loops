

# Exercises: JavaScript loops

Paste your answers into this file.

<br>

## Print every number from 0 to 10

```
for(let i = 0 ; i <= 10 ; i++){
console.log(i);
}
```

<br>

## Print every number from 10 to 0

```
for(let i = 10 ; i >= 0 ; i--){
console.log(i);
} 
```

<br>

## Print every number from 4 to -16

```
for(let i = 4; i <= 16 ; i++){
console.log(i);
}
```

<br>

## Print every fifth number from 8 to 41

```
for(let i = 8; i <= 41 ; i+=5){
console.log(i);
}
```

<br>

# Exercises: JavaScript loops with array:

Paste your answers into this file.



1. Change all **odd** numbers to be those numbers multiplied by two:
```js
const numbers = [4, 9, 7, 2, 1, 8];

  // your code here
  for(let i = 0; i< numbers.length ; i++){
    if(numbers[i] % 2 === 1){
console.log(numbers[i]*2);
    }else
console.log(numbers[i]);
  }

numbers; // => [4, 18, 14, 2, 2, 8]
```

2.  Create an array to hold your favorite colors.  For each choice, log to the screen a string like: `My #1 choice is blue.`

const colors = ["blue","black", "pink" ];
for(let i = 0 ; i <=colors.length; i++){
console.log("My #"+ i +" choice is "+ colors[i]);
}
3.  Create an array of ages.  Loop through and log only the ages that are over 21.
const ages = [18,21,19,23,15];
for(let i = 0 ;i <= ages.length; i++) {
if(ages[i] > 21){
console.log(ages[i]);
}
}
1. Create an array to hold your top five choices of something (music, books, movies, whatever).
 
    - For each choice, log to the screen a string like: "My #1 choice is blue."
    - **Bonus:** Change it to log "My 1st choice, "My 2nd choice", "My 3rd choice", picking the right suffix for the number based on what it is.
    
const choice = ["anime","video game","music","movies","books"];
const  suffixNumber= function(array){
for(let i = 0; i<= array.length;i++)
{
 
if (i === 1 ) {  
    console.log("My "+i+"st choice "+array[i]);
 }
else if (i === 2) { 
    console.log("My "+i+"nd choice "+array[i]);
 }
else if (i === 3  ) { 
    console.log("My "+i+"rd choice "+array[i]);
 }
else {
    console.log("My "+i+"th choice "+array[i]);
 } 

}

}

## The classic Fizzbuzz Program

For every `number` between 1 and 100...

If the `number` is evenly divisible by 3, print "Fizz"

If the `number` is evenly divisible by 5, print "Buzz"

If the `number` is evenly divisible by 3 AND evenly divisible by 5, print "Fizzbuzz"


```
for(let num =1 ; num <= 100;num++){
if (num % 15 === 0 ) {  
    console.log("FizzBuzz") }
else if (num % 5 === 0) { 
    console.log("Buzz") }
else if (num % 3 === 0 ) { 
    console.log("Fizz") }
else {
    console.log(num) } 

}

  ```

<br>


## The even/odd reporter

Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen (e.g. "2 is even").

```
for(let i = 0; i<=20 ;i++){
if(i % 2=== 0){
console.log(i+" is even ");
}else {
console.log(i+" is odd ");

}
}
```

<br>

## Multiplication Tables

Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result (e.g. "2 * 9 = 18").

Bonus: Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).


```
let result = '';
for(let i = 0; i <=10; i++){
result = i*9;
console.log(i+" * 9 = "+result);
}
//Bonus 
let result = '';
for(let i = 0; i<= 10;i++){
  for(let j = 0; j<= 10;j++){
result = i * j;
  console.log(i+" * "+ j +" = "+result);

  }
}
```

<br>

## The Grade Assigner

Check the results for every value from 60 to 100 - so your log should show "For 89, you got a B. For 90, you got an A.", etc.

```

  for(let grade = 60;grade <=100;grade+=10){
  if(grade >= 90){
console.log(grade +" You got an A.");
  }else if(grade >= 80){
console.log(grade +" You got an B.");
  }else if(grade >= 70){
console.log(grade +" You got an C.");
  }else if(grade >= 60){
    console.log( grade+" You got an D");
  }
  else {
   
console.log(grade +" You got an F");
  
  }
  }

```
