# JavaScript

js always linked at bottem of body so it loads last.



array stores informoation by index/postion/order

 let objects = {}
 let arrays  = []
let strArr = ['howdy', "hello"]
let numArr
let mixArr= ['5', 20, ['sup']] 
<!-- try t0 avoid mixed type arrays -->



<!-- objects stores infomoration by key vlaue pair -->
let objects = {
  <!-- provide the key obj. would give same value, objects does not contain a predicblte order. no order in key they ran if order matters dont use object-->
  key: " value ",
  name: "moath",
  costume: none,


<!-- stores infomoration by key value pair -->
let person key{
 key: " value ",
  name: "moath",
  costume: none,
}

  reference types, create a link between values


function doSomething(){
  
}
<!-- function empty brackets would grab function data. Functions run when you want them to. -->

let blank = function (){

}

<!-- concepts for futures -->

let funcArr = [funky]




function  returnSum () {

  return 'something' 
  <!-- returns value from function to where the function was called -->
}

<!-- let result = something
result = something -->
<!-- take values from function, to give back to the caller. -->
function sum (){
  return 5+10
}


to link to js

in html 

onblur'
onfoucs focuses
ondrag
ondragStart
ondragstop

onClick = "doSomething()"



<!-- you can only add strings together -->



<!-- if your changing data console log the data -->

function submit() {
  let isCodeCorrect = yourCode == secertcode
  log iscodecorrect
  if ( is codecorrect)
  log  correct
   else {
   log incorrect
   }
}

drawCode() replaces the actaul codee from the id
let blankElm = document.getElementById ("id?")


add draw code every function 
tell functiom to go thorugh it


<!-- debugger pasure your code in actions to watch chnages happen.. -->



<!-- objeccts and arrys -->

dont write undefined as value

instead use null = no value

you select data from array from the postion

you can do an array within an array within an array

data can be chained togather.


<!-- stater          comparison         afterthought -->
<!-- rhw start,    the end,    the speed or incremantion-->
for (let index =1: index <= 10: index++){
  log ('looped', index)
}



for loops can iteratte over arrays or sets of data

add an length behind array

for (let index = 1; index <= catArr.length; index ++){}

if index is same or less then array, remove <


const element = array [index]


const  define a value that can be changed

goood use of const is itterating over an array.



methods are functions that stick like a class, functions for you to utilize

function and methods are yellow

foreach (() =>)

prectnetses arrow is a function that does not have a name

for each does it once

for loops  can be done more
for loop inside a for loop


<!-- cat alias for element of array, (i) index of this element -->
catArr.foreach(() = > log (cat, i, 'for each'))

<!-- returns the value of the first element in the array where predicae is true and undeifned other
find takes in a function,  -->
catArr.find() 
<!-- find grts refernce to a single element of the arry to operate on. -->
log ( logo 'found' cat arr.find (cat => cat.name == 'fido'))

<!-- find, finds the first whre this is true -->
let foundByage = catArr.find(cat => cat.age > 5)
log "found", foundByAge

<!-- returns the elemnts of an array that meet the condtion specifed in the call back -->
<!-- filter, creates a new array where it keeps all the ture items. -->
let lastLives = catArr.filter(cat => cat.livesleft == 0)
log "filtered" last lives


let oldestCatNoLives = lastLives.find(cat => cat.age > 5)


let olderCats = catArr.filter(cat => cat.age > 7)
log  "filtered older;", oldercat



<!-- compare 0 to 1 and 1 to 2 -->
let sortedCats = catArr.sort ((cat2, cat1) => cat1.age - cat2-age)

<!-- array methods itterate over -->


<!-- find, finds what you need it to find -->

<!-- sorts orders the array based in postive or negative values being teturned from the funcyion  -->

<!-- functions can take in arguments/parameters -->

<!-- aniamls is full aray a and b = postion of the array.. -->

includes is an array method that returns true or false if that array inculdes the thing

! 

join a string used to seperate one element  if the array frim the ne



? = eqauls is this true or false

? " a mamal " : 'not a mamal'

if its true choose 1, if not choose 2.

strings snap in together

innertext can also be innerhtml 


