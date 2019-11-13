## Task 1

### 1.1
```
var letters = [];
var weather = "The weather is nice".split(" ");
for ( var a = 0; a < weather.length; a++ ) {
	letters.push( weather[a][0] );
}

console.log ( letters );
```

### 1.2
```
var str = letters.join("");
console.log (str);
```

## Task 2

### ver1
```
function checkNmbr (x) {
    if ( typeof(x) !== "number" ) 
    	console.log ( "Неверный тип данных" )
    else 
	console.log (new Date().toLocaleString());
}

checkNmbr (2) //проверяем с числом
checkNmbr ("a") //проверяем с не числом 
```

### ver1
```
function checkNmbr (x) {
    if ( typeof(x) !== "number" ) 
    	return "Неверный тип данных"
    return (new Date().toLocaleString());;
}

checkNmbr (2) //проверяем с числом
checkNmbr ("a") //проверяем с не числом 
```

## Task 3

Ставим точку останова:
[**Screen1**](https://prnt.sc/pw51j0)

Смотрим как работает вредоносный код:
[**Screen2**](https://prnt.sc/pw51te)

Меняем в файле index01.js код 
```
return userText
```
на 
```
return userText.split("<").join("&lt;")
```
и обезвреживаем вредоносный код:
[**Screen3**](https://prnt.sc/pw52li)


