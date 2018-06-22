# Basic-Algorithm-Scripting-Title-Case-a-Sentence
```
function titleCase(str) {
  var a= str.toLowerCase();
  var b= a.split(" ");// ["i'm", "a", "little", "tea", "pot"]
      for(var i=0; i< b.length; i++){
      b[i] = b[i].charAt(0).toUpperCase() + b[i].slice(1);
 }// charAt(0) là nhặt phần tử đầu của chuỗi rồi viết hoa + lát cắt các phần tử từ thứ 1 của các chuỗi.
   var text = b.join(" ");
       return text;
 }
 titleCase("I'm a little tea pot");
```

# Repeat-a-String-Repeat-a-String
```
function repeatStringNumTimes(str, num) {
  var text="";
for(var i=0 ; i<num ; i++){
  text += str;
}
  return text;
}

repeatStringNumTimes("abc", 3);
```

# Confirm-the-Ending
```
function confirmEnding(str, target) {

var a= str.lastIndexOf(target);//6-tìm chuỗi target trong str ở vị trí cuối
var b= str.length;//7
var c= a+ target.length;//6+1
var d= c==b;
  return d;
}
confirmEnding("Bastian", "n");
```
# Truncate-a-String
```
function truncateString(str, num) {
  // Clear out that junk in your trunk
  var text="";
  var a= str.slice(0,num);
  if(str.length > num){text= a +"...";}
  else{text=a;}
  return text;
}
truncateString("A-tisket a-tasket A green and yellow basket", 8);
```
#  Where do I Belong  
```
function getIndexToIns(arr, num) {
  // Find my place in this sorted array.
arr.push(num); // thêm num vào mảng arr
arr.sort(function(x,y){return x-y}); // sắp xếp thứ tự của mảng arr
var a = arr.indexOf(num); //xác định vị trí của num trong mảng arr
  return a;
}
getIndexToIns([40, 60], 50);
```
#  Mutations
```
function mutation(arr) {
var a= arr[0].toLowerCase().split(""); // ["h", "e", "l", "l", "o"]
var b= arr[1].toLowerCase().split(""); // ["h","e","y"]

for(var i =0; i < b.length; i++){
  b[i] = a.indexOf(b[i])// [0,1,-1]
}
var c= Boolean(b.indexOf(-1)==-1); // tìm kiếm xem -1 có trong b không, nếu có thì là false
  return c;
}
mutation(["hello", "hey"]);
```
# Chunky Monkey  
```
function chunkArrayInGroups(arr, size) {
  // Break it up.
var text = [];
  for(var i=0 ; i < arr.length ; i += size){
    text.push(arr.slice(i , i + size));
}
  return text;
}
chunkArrayInGroups(["a", "b", "c", "d"], 2);
```
