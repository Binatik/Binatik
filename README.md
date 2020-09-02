# Serega Mangushev  
Junior WEB-разработчик, Россия.  

[TOCM]

# Skills 
### html/css
#### HTML
```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Skills</title>  
        <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no"> 
        <link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,700;1,500&display=swap"
    rel="stylesheet">
        <meta name="description" content="skills html">  
        <link rel="stylesheet" href="./src/styles.css"> 
    </head>
<body>
    <main class="page">
        <section class="page__product product center-items"> 
		<h2 class="product__title">HTML</h2>
            <div class="row wrapper">
                <div class="product__item col3">
                    <h3 class="product__subtitle">HTML - Skills</h3>
                    <img src="#" alt="test">
                    <p class="product__text">Высокий уровень знаний чистого HTML.</p>
                </div>
                <div class="product__item col3">
                    <h3 class="product__subtitle">CSS - Skills</h3>
                    <img src="#" alt="test">
                    <p class="product__text">Отличные навыки стилей..</p>
                </div> 
            </div>
        </section>
    </main>
    <script src="#"></script>
</body>
</html>
``` 

#### CSS - first level
```css
* {
    scroll-behavior: smooth;
    box-sizing: border-box;
    padding: 0;
    margin: 0;
    font-size: 100%;
    border: 0;
    outline: none;
}

body,
html {
    overflow-x: hidden;
} 

.center-items {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
} 

.wrapper {
    width: 100%;
    padding: 15px;
    max-width: 1280px;
    margin: 0 auto;
}
```  
 
#### CSS - second level
```css
.page__product {
    padding: 50px 0;
}

.product__title {
    font-size: 34px;
    color: #000;
    letter-spacing: 2px;
}

.row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.product__item {
    flex: 1 33.333%;
    padding: 15px;
    margin: 15px;
    background-color: #fff;
    box-shadow: 4px 2px 24px -8px rgba(0, 0, 0, 1);
    border-radius: 5px;
} 

.product__subtitle {
    font-size: 22px;
    color: #000;
}

.product__text {
    font-size: 18px;
    color: #000;
}
``` 

#### CSS - third level
```css
.product__item {
    position: relative;
    transition: 0.2s;
}

.product__item:hover {
    transform: translateY(5px);
}

.product__item:before {
    position: absolute;
    left: 0;
    top: 0;
    content: '';
    width: 100%;
    height: 10px;
    background-color: #000;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
}
``` 
#### Посмотреть: 
[![](https://hostadvice.com/wp-content/uploads/2017/04/codebox-logo-e1595399885122.png)](https://codesandbox.io/s/htmlcss-dso9f?file=/index.html "Открыть в редакторе.") 

### JavaScript
#### Array() 
```js
const elements = ["El1", "El2", "El3"]; //Просто
const numbers = [1, [5, [9, 8, 7], 7], 3]; //Сложно
```  

#### Object()
```js
const Test = { test: "0", test: "1", test: "2" }; //Просто
const Color = [{ red: "Red" }, { green: "Green" }, { test: "Test" }]; //Обычно
const Product = [
  {
    title: "Test - 1",
    price: 1,
  },
  {
    title: "Test - 2",
    price: 2,
  },
  {
    title: "Test - 3",
    price: 3,
  },
  {
    title: "Test - 4",
    price: 4,
  },
]; //Сложно

```  

#### jsx
```js  
//Уточнение: Пример написан на языке javaScript - шаблонные строки.
` 
    <h3 class="product__subtitle">${subtitle}</h3>
    <img src="#" alt="test">
    <p class="product__text">Зарплата от ${number}</p> 
`; 
```

#### function
```js
//Function Expression
function sum(a, b) {
  return a + b;
} 

//Function Declaration
sum = (a, b) => a + b;


//Function callback
function sum(a, b) {
  return function(){ 
    a+b
  }
} 
 
/* 
Примечание callback - это функция обратного вызова.  
Такая функция может быть вызвана в другой функции.  
На сегодня  javaScript  без callback может умереть.  
Многий функционал освоен именно на них.  
Для примера мы можем взять цикл forEach,  
куда обязательно нужно передавать callback.
*/
```  
#### inline function + callback
```js
/* 
Примечание - reduce необходимо установить параметр в качестве 0, 
если вы пытаетесь сложить свойство у ключей допустим.  
Опустите данный параметр, если массив обычный,  
типа [1,2,3,4,5] - подсказка, вы можете таким образом получить сумму данного массива.
*/
arr.reduce((acc, current) => acc + current, 0); //acc = 0;  
arr.forEach((element, i) => element + '' + i); 
arr.sort((a, b) => a-b);  
/* 
Примечание - Некоторые функции типа  map возвращают результат в новый массив,  
при этом состояние  родителя не изменилось 
*/ 
const newArr = arr.map((current,i) => current + i)
```   

#### async + promise
```js
const promise = new Promise((resolve, reject) => {
  resolve("Этот текст вернет resolve - т.е promise");
  reject("Если произошла ошибка");
});

/*       
Примечание - then() - Это метод.  
Подсказка -  возвращает Promise.  
Уточнее: then() является одним из методов экземпляра класса Promise. 
*/
promise.then((promise) => console.log(promise));
promise.then((promisetext) => console.log(promisetext + "text"));
promise.then((promisetextContent) =>
  console.log(promisetextContent + "textContent")
); 

//Function
let global;
function getData(text) {
  return new Promise((resolve, reject) => {
    resolve(text);
    reject("Если произошла ошибка");
  });
}

/*
Примечание - Функция getData возвращает экземпляр Promise. 
Подсказка - вам доступны у данной функции все методы, что и у примера выше  
Внимание - Вам необходимо вернуть состояние в данном примере,  
если этого не сделать, вернется undefined.
*/
getData("Этот текст вернет resolve - т.е promise") 
  .then((test) => {
    global = test;
    console.log(global);
    //Возможный вызов функции. 
    return global;
  })
  .then((testNumber2) => {
    global = testNumber2 + 'NewPromise';
    console.log(global);
    //Возможный вызов функции.
  })  
/* 
Уточнее - Вернуть состояние можно как значение или как new Promise((resolve, reject) 
*/
```  