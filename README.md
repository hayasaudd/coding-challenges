# Coding Challenges

## 1st Challenge
Create a function that receives an integers array and returns the number that appeared only once.

| Input           | Output   |
| --------------- | -------- |
| (2,4,6,4,9,6,2) | 9        |
| (1,1,2)         | 2        |
| (2,2,1)         | 1        |

##Answer
   val arry: IntArray = intArrayOf(2,4,6,4,9,6,2) 
   var iterNum = arry.toList()
   var x =iterNum[0]
   for (index in iterNum.length()){
       if (x == iterNum[index]){
           x= iterNum[index]
       }
   }
   println(x)
   
   this answer for bigest number 
   /*answer:
val list1= listOf(2,4,6,4,9,6,2)
var bigNum = list1.maxOrNull()
println(bigNum)
*/

## 2nd Challenge
Create a function that receives a string then it converts uppercase letters into lowercase and vice versa. The function then should print the converted value.

| Input          | Output         |
| -------------- | -------------- |
| Hello          | hELLO          |
| Hi             | hI             |
| Hello World    | hELLO wORLD    |
| My name is Ali | mY NAME IS aLI |
| sHroog         | ShROOG         |


## 3rd Challenge
Create a function that receives an array of items & arrays and returns one flattened array with all items exluding null values.

| N | Input                                 | Output                |
| - | ------------------------------------- | --------------------- |
| 1 | [1,[2,3,null,4],[null],5]             | [1,2,3,4,5]           |
| 2 | [7, 0,[null],[null, null, 9]]         | [7, 0, 9]             |
| 3 | [[null, 3], [2, 4, 5, null], 0, 8, 3] | [3, 2, 4, 5, 0, 8, 3] |
| 4 | [3, 5, [5, 9, 0]]                     | [3, 5, 5, 9, 0]       |

val list1= listOf(2,4,6,4,9,6,2)
var nullElement = list1.map (if (this == null){list1.remove(this)})


## 4th Challenge
Create a function that receives a string that contains combination of parentheses, square brackets, and curly braces. Then, it returns true if every opening bracket has a closing pair.

| Input    | Output |
| -------- | -------- |
| }{       | false    |
| ()       | true     |
| )({}     | false    |
| ({ }})   | false    |
| ({ })    | true     |
| {{()}}   | true     |
| {{()}    | false    |
| [{}]     | true     |
| {[(}])   | true     |
| {[}])    | false    |



