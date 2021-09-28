1) var user = {name:'Peter',printMessage(){console.log(`Hello ${this.name}`)}}; var printMessage = user.printMessage; printMessage()
   Hello John

2)  console.log(message)
    let message = 'Hello'
    Error Возникнет ошибка

3)  for(var i =0; i<10;i++){
  ///
}
console.log(i) => 10

4) 'use strict'
    const details = {
        message:'Hello',
    }
    function getMessage(){
      return this.message;
    }
    console.log(getMessage.call(details))
    'Hello'

5) for (let i =0;i <3;i++){
  setTimeout(function(){
    console.log(i)
  },1000)
}
  0,1,2

6)  function foo(a,b){
      return a*b
    }
    const bar = foo.bind(null,2)
bar(2)
  4

7) Что такое замыкание?
    Способность функции запоминать переменные из внешней области видимости в момент ее создания

8)  Какие варианты правильно объявляют функцию f, возвращающую сумму двух аргументов?
    let f = function(a,b) { return a+b }

    let f = new Function("a,b", "return a+b")

    let f = new Function("a", "b", "return a+b")

    let f = (a, b) => a + b
9)  const foo =bar()
    const nuber = 2;
    function bar(){ return number}

    undefined

10)  Укажите правильный способ получения доступа ко всем аргументам функции
      
      function foo(){
        console.log(arguments)
      }

11)   Что будет выведено в консоль?
      function foo(){
        return {bar:'1'}
      }
      console.log(typeof foo().bar)

      String
12) (
        function(a){
          arguments[0] = 10
          return a;
        }
    )(5)
  10

13) console.log(message)
    var message = 'Hello'
    undefined

14) printMessage()
    function printMessage(){
      console.log('hello')
    }
    hello
15) var a = 1; b = function a(x) { x&& a(--x);}
    1

16) var name = 'John'
    function printName(){
      console.log(name)
      var name = 'Peter'
      console.log(name)
    }
    printName()

  undefined 'Peter'

17) for(var i=0; i<3; i++){
    setTimeout(function(){
      console.log(i)
      },1000)
    }
  3

18) Каким образом осуществляется передача параметров в функцию?
    
  Примитивы передаются по значению, а объекты - по ссылке

19) let name = 'John'
    function printName(){
      console.log(name)
      let name = 'Peter'
      console.log(name)
    }
    printName()

Возникнет ошибка

20)  'use strict'
      function getThis(){ retur this; } 
      console.log(getThis())

undefined

21)  function foo(){ console.log(this)}
foo.call(null)

window

22)  
    const details = {
        name:'John',
    }
    function getMessage(){
      return `${message}  ${this.name}`;
    }
    console.log(getMessage.apply(details,['Hello']))
    
'Hello John!'

23) let f = function g(){return 23}; console.log(typeof g())
    Возникнет ошибка
24) function getThis(){ return this;} 
    console.log(getThis())

25) let name ='John'
function printName(){
  console.log(name)
}
setTimeout(()=>{
  let name ="Peter"
  printName()
},1000)
john

26)Укажите, что в JavaScript подвергается всплытию (hoisting)?
Function expression
Function declaration
Объявление переменной

  JS Scope & Functions 85%
