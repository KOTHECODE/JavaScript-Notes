# JavaScript-Notes
JAVASCRIPT NOTES

            <!DOCTYPE html>
            <html lang="en">
            <head>
                <meta charset="UTF-8">
                <meta name="viewport" content="width=device-width, initial-scale=1.0">
                <link rel="stylesheet" href="style.css">
                <title>Document</title>
            </head>
            <body>
               
                <script src="index.js"></script>
            </body>
            </html>



            
            //This is a Comment 
                                 
           /*
           this is 
           a 
           comment 
           */


           console.log('Hello World');
           window.promt('propmt some sort of input');
           window.alert('This is an alert!');


           First must declare an ID in html 
           document.getElementById('myH1').textContent = 'Hello My People';
           document.getElementById('myP').textContent = 'Lets all learn to code together ';



***** Variable = a container that stores a value. *****
           Behaves as if it were the value it contained 

           1. declaration  let x;
           2. assignment   x = 100;

              let x = 123;

***** Data Types: *****

    Numbers::
        let age = 23;
        let price = 10.99;
        let gpa = 3.9;

            console.log(typeof gpa);
            console.log('You are ${age} years old');
            console.log('The price is ${price}');
            console.log('Your gpa is: ${gpa}');

    Strings::  ('a series of characters')
        let firstName = 'Bro';
        let favoriteFood = 'pizza';
        let email = 'ornisk123@yahoo.com';  (these numbers cannot be used for math)

            console.log(typeof firstName);
            console.log('Your name is  ${firstName}');
            console.log('you like ${favoriteFood}');
            console.log('Your email is  ${email}');

    Boolean::  ('True or false ')
        let online = false;
        let forSale = true;
        let isStudent = true;

            console.log('Bro is online ${online}');
            console.log('Is the car for sale ${forSale}');
            console.log('Enrolled: ${isStudent}');



***** Arithmetic Operators = operands (values, variables, etc.) *****

           operators (+ - * /)
           ex. 11 = x + 5;

        Let students = 30;

        students = students + 1;
        students = students - 1;
        students = students * 1;
        students = students / 1;
        students = students ** 1;
        let extraStudents = students % 3;

            or 

        students += 1;
        students -= 1;
        students *= 1;
        students /= 1;
        students **= 1;
        let extraStudents %= 3;

        student++;  (gives you students plus 1 )
        student--;  (gives you students minus 1 )
        

            console.log(students);

  *****  Operator precedence *****
  
        1. Parenthesis ()
        2. exponents
        3. mulitplication and division and modulo
        4. addition and subtraction 
        
    Example:
        let result = 1 + 2 * 3 - 4 ** 2;
            consol.log(result);



***** How to Accept user Input *****

    1. Easy way = Window Prompt 
        let username ;
            username = window.prompt('whats your username?');
            console.log(username);

    2. PROFESSIONAL WAY = HTML textbox 
        let username;
        document.getElementById('mySubmit').onclick = function(){
            username = document.getElementById('myText').value;
            document.getElementById('myH1').textContent = 'Hello ${username}'
        }

***** Type Conversion = Change the datatype of a value to another *****
                  (strings, numbers, booleans)

                let x = '10';
                let y = '10';
                let z = '10';

                            x =  Number(x);
                            y =  String(y);
                            z =  Boolean(z);

***** const = a variable that cant be changed *****



***** Math = built-in object that provides a collection of properties and methods. *****

           let x = 30;
           let y = 2;
           let z;
                      z = Math.round(x);
                      z = Math.floor(x);
                      z = Math.ceil(x);
                      z = Math.trunc(x);
                      z = Math.pow(x, y);
                      z = Math.sqrt(x);
                      z = Math.log(x);
                      z = Math.sin(x);
                      z = Math.cos(x);
                      z = Math.tan(x);
                      z = Math.abs(x);
                      z = Math.sign(x);
                                 console.log(z);
                      
                          
                      let max = Math.max(x, y, z);
                      let max = Math.min(x, y, z);
                                 console.log(max);
                                 console.log(min);

***** IF STATEMENTS = if a conditon is true, execute some code if not, do something else *****

           if(condition){
                      Action
                      console.log('message');
           }
           else{
                      if the if condition is not true then do this this
                      console.log('message');
           }

== two equal signs check if equal to 
           
***** CHECKED = property that determines the checked state of an HTML checkbox or radio button element *****


***** TERNARY OPERATOR = a shortcut to if{} and else{} statements helps to assign a varibale based on a condition (better then using IF/Else statements)*****
                   condition ? codeIfTrue : CodeIfFalse;
                   
           Example: let age = 21;
                    let message = age >= 18 ? 'you're an adult' : 'your a minor';
                    console.log(message);
                    
***** SWITCH = can be an efficent replacement to many Else/If statements *****

           Example 1:
                      let day = 1;
           
                                 switch(day){
                                     case 1:
                                          console.log('It is Monday!');
                                          break;
                                     case 2:
                                          console.log('It is Tuesday!');
                                          break;
                                     case 3:
                                          console.log('It is Wednesday!');
                                          break;
                                     case 4:
                                          console.log('It is Thursday!');
                                          break;
                                     case 5:
                                          console.log('It is Friday!');
                                          break;
                                     case 6:
                                          console.log('It is Saturday!');
                                          break;
                                     case 7:
                                          console.log('It is Sunday!');
                                          break;   
                                     default:
                                                console.log(${day} is not a day!');
                                                
                                 }

           Example 2:
           
                      let testScore = 71;
                      let letterGrade;
                                 
                                 switch(true){
                                     case  testScore >= 90:
                                            letterGrade = 'A';
                                            break;
                                     case  testScore >= 80:
                                            letterGrade = 'B';
                                            break;
                                     case  testScore >= 70:
                                            letterGrade = 'C';
                                            break;
                                     case  testScore >= 60:
                                            letterGrade = 'D';
                                            break;
                                     default:
                                            letterGrade = 'F';
                                 }
                                 console.log(letterGrade);

***** STRING METHODS = allow you to manipulate and work with text (strings) *****

      Example:
           let userName = 'BroCode';

           console.log(userName.charAt(0));
           console.log(userName.indexOf('o'));
           console.log(userName.length);
           
           userName = userName.toLowerCase();
           userName = userName.toUpperCase();
                      console.log(userName);

***** METHOD CHAINING = Calling one method after another in one continuous line of code. *****

           let userName = Window.prompt('Enter your username: ');

           ----- NO METHOD CHAINING ------

           userName = userName.trim();
           let letter = letter.chartAt(0);
           letter = letter.toUpperCase();

           let extraChars = userName.slice(1);
           extraChars = extrachars.toLowerCase();
           userName = letter + extraChars;

           console.log(username);

           ----- Method Chaining -------

           userName = userName.trim().chartAt(0).toUpperCase() + userName.trim().slice(1).toLowerCase();
           console.log(userName);

***** LOGICAL OPERATORS = used to combine or manipulate boolean values (true or false) *****

           AND = &&
           OR = ||
           NOT = !
           
    Example:
           const temp = 20;

           if(temp > 0 && <= 30){
                console.log('the whether is good');
           }
           else{
                console.log('the weather is bad');
           }

           ------ OPERATORS -----   

                      = assignment Operator 
                      == comparison operator (compare if values are equal)
                      === strict equality operator (compare if values & datatype are equal)
                      != inequalify operator
                      !== strict inequality operator 



***** WHILE LOOP = repeat some code while some condition is true *****

           Example: 
                      let userName = '';

                                   while (userName === '' || userName === null){
                                              userName = window.prompt ('enter your name');
                                   }
                                   console.log('Hello ${userName}');


***** FOR LOOP = repeat some code a LIMITED amount of times *****


     Example: 
           for(let i - 0; i <= 10; i++){
                      console.log(Hello);
                      console.log(i);
           }

****** Function = a section of reusable code. (declare once, use it whenever you want. Call the function to execute that code.) ********   

    Example 1: 
           function happyBirthday(username, age){
                      console.log('HAPPY BIRTHDAY TO YOU!!!');
                      console.log('HAPPY BIRTHDAY Bro!!!');
                      console.log('HAPPY BIRTHDAY DEAR ${username}!!!');
                      console.log('HAPPY BIRTHDAY YOU ARE NOW ${age} YEARS OLD!!');
                      }
           happyBirthday('kim', 28);
           happyBirthday('spongebob', 50);
           happyBirthday('patrick', 29);

    Example 2: 
           function add(x, y){
                      return x - y;
                      }
           function subtract(x, y){
                      return x - y;
                      }
           function multiply (x, y){
                      return x * y;
                      }
           function divide (x, y){
                      return x / y;
                      }
                      
           console.log(add(2, 3));
           console.log(subtract(2, 3));
           console.log(multiply(2, 3));
           console.log(divide(2, 3));
