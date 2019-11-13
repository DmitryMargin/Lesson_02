```
# 1.1
var letters = [];
var weather = "The weather is nice".split(" ");
for ( var a = 0; a < weather.length; a++ ) {
	letters.push( weather[a][0] );
}

console.log ( letters );

# 1.2
var str = letters.join("");
console.log (str);
```
```
# 2.var1
function checkNmbr (x) {
    if ( typeof(x) !== "number" ) 
    	console.log ( "Неверный тип данных" )
    else 
	console.log (new Date().toLocaleString());
}

checkNmbr (2) //проверяем с числом
checkNmbr ("a") //проверяем с не числом 

# 2.var2
function checkNmbr (x) {
    if ( typeof(x) !== "number" ) 
    	return "Неверный тип данных"
    return (new Date().toLocaleString());;
}

checkNmbr (2) //проверяем с числом
checkNmbr ("a") //проверяем с не числом 
```
