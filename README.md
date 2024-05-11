<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <div id="const"></div>
    <script>

        var x = 10;
         x *= 5;
        x /= 2;
        x -= 3;
        x += 7;

        document.getElementById("object").innerHTML = x;

        let text1 = 10;
        let text2 = 5;
        let result = text1!=text2;
        document.getElementById("comp").innerHTML = "text1 is greater than text2" + result;

        let x = 5;
        let y = 7;

        document.getElementById("logic").innerHTML = 

        (x > 3 && y < 5) + "<br>"
        !(x > 10);


        let result;
        let age = 15;
        if (age >= 18)
        {
            result = "you are old enough for vote";
        } 
        else
         {
            result = "you are not old enough for voting";
        }

        document.getElementById("if-else").innerHTML = result;
        let output = document.getElementById("else-if")
        let book = "english";
        if (book == "maths")
        {
            output.innerHTML = "you are reading maths book";
        }
        else if (book == "science")
        {
            output.innerHTML = "you are reading science book";
        }
        else if (book == "history")
        {
            output.innerHTML = "you are reading history book";
        }
        else
        {
            output.innerHTML = "you are reading a book";
        }

        let month;
        switch (new Date().getMonth()){
            case 0:month = "january";
                break;

            case 1:month = "feburary";  
                break;

            case 2:month = "march";
                break;   

            case 3:month = "april";
                break;    

            case 4:month = "may";
                break;

            case 5:month = "june";
                break;

            case 6:month = "july";
               break;

            case 7:month = "august";
               break;

            case 8:month = "september";
               break;

            case 9:month = "october";
               break;

            case 10:month = "november";
               break;

            case 11:month = "december";
               break;   
        }

        document.getElementById("switch").innerHTML = "this month is" + month;

        let person = {
            firstName: "saira",
            lastName: "ghulam hussain",
            id: 1525935,
            fullName: function (){
                return this.firstName + " " + this.lastName + " " + this.id;
            }
        }
        document.getElementById("this").innerHTML = person.fullName();


        function person(first, last, age, eye) {
            this.firstName = first;
            this.lastName = last;
            this.age = age;
            this.eyeColor = eye;
            this.name = function () {
                return `My father name is ${this.firstName} ${this.lastName} his age is${this.age} and his eyescolor is ${this.eyeColor}`
            }
        }
        
        const myFather = new person("Ghulam", "Hussain", 60, "brown");
        document.getElementById("const").innerHTML = myFather.name();
        


        function person(first , age , aptech ,){
            this.firstName = first;
            this.age = age;
            this.aptech =  aptech;
            this.details = function (){
                return `I am ${this.firstName} <"br"> i am ${this.age} years old <"br"> i study in ${this.aptech}`
            }
        }

        const myself = newperson("saira" , "21" , "aptech");
        document.getElementById("const").innerHTML = myself.details();
        </script>
</body>

</html>
