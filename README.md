# Assignment-2



#Q2 Answer
#HTML
<!DOCTYPE html>
<html>
<head>
<meta charset=utf-8 />
<title>mycolor</title>
</head>
<body>
</body>
</html>

#JS
myColor = ["Red", "Green", "White", "Black"];
console.log(myColor.toString());
console.log(myColor.join());
console.log(myColor.join('+'));





#Q4
#HTML
<!DOCTYPE html>
<html>
<head>
<meta charset=utf-8 />
<title>Write a JavaScript program to find the most frequent item of an array. - w3resource</title>
</head>
<body>
</body>
</html>

#JS
var arr1=[3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3];
var mf = 1;
var m = 0;
var item;
for (var i=0; i<arr1.length; i++)
{
        for (var j=i; j<arr1.length; j++)
        {
                if (arr1[i] == arr1[j])
                 m++;
                if (mf<m)
                {
                  mf=m; 
                  item = arr1[i];
                }
        }
        m=0;
}
console.log(item+" ( " +mf +" times ) ") ;



Q5
#HTML
<html>
<head>
<meta charset=utf-8 />
<title>JS Bin</title>
<style>
body {padding-top:50px} 
</style> 
</head>
<body>
<input type="text" id="text1"></input>
<input type="button" id="button1" value="Add" onclick="add_element_to_array();"></input>
<input type="button" id="button2" value="Display" onclick="display_array();"></input>
<div id="Result"></div> 
</body>
</html>



#JS
var x = 0;
var array = Array();

function add_element_to_array()
{
 array[x] = document.getElementById("text1").value;
 alert("Element: " + array[x] + " Added at index " + x);
 x++;
 document.getElementById("text1").value = "";
}

function display_array()
{
   var e = "<hr/>";   
    
   for (var y=0; y<array.length; y++)
   {
     e += "Element " + y + " = " + array[y] + "<br/>";
   }
   document.getElementById("Result").innerHTML = e;
}
