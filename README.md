# Basic-Algorithm-Scripting-Title-Case-a-Sentence

### function titleCase(str) {
###   var a= str.toLowerCase();
###   var b= a.split(" ");// ["i'm", "a", "little", "tea", "pot"]
###       for(var i=0; i< b.length; i++){
###       b[i] = b[i].charAt(0).toUpperCase() + b[i].slice(1);
### }// charAt(0) là nhặt phần tử đầu của chuỗi rồi viết hoa + lát cắt các phần tử từ thứ 1 của các chuỗi.
###   var text = b.join(" ");
###       return text;
### }

### titleCase("I'm a little tea pot");
