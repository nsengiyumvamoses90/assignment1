# assignment1
this my coding  tutorial
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Document</title>
    <style>
        #part1{
            border: none;
            padding: 0 30px;
            font-size:16px;
            font-weight: 500;
            border-bottom: 2px solid rgba(0, 0, 0, 0.2);
            
    
        }
        #part3{
            margin-top: left;
            padding: 0;
            list-style: disc;
            text-outline: 0 0 rgb(226, 19, 19);
        }
        #part2{
            display: flex;
            position: absolute;
            z-index: 111;
        }
        #part{
            height: 100%;
            width: 100%;
            display: flex;
        }
    </style>
</head>
<body>
    
<div class="container">
    <form action="#">
    <div class="input-boxes">
      <h1 style="size: 40px;";>Fill the form.</h1>
      <h1>It's easy.</h1>
        <div class="former-content">
            
             <input type="text" name="first name" value="First name" id="part1">
            
              
              
              <input type="text" name="last name" value="Last name" id="part1"><br><br>
              
               
             <input type="email" name="email" value="Email" id="part1"><br><br>
            
             
            
            
             <p>Briefly tell about project and your current goals</p>
                
                <p>How can we help you?</p>
                <input type="textarea" name="textarea" value="" id="part1"><br><br>
    
                <button  class="message">send message</button>
                
            
            
                <h4 id="part2">Need presentation?</h4>
                <p id="part2">You like what we do but you need 
                    to demonstrate your team as well Easy Directly download, print
                     or share the link to a PDF with your collegues</p>
                     

            </div>
        </div>
            
    </div>



        </form>

    
    
</body>
</html>
//css style
body{
    min-height: 100vh;
    display:flex;
    align-items: center;
    justify-content: center;
    padding: 30px;
    
    ;
}
.container{
    border: 1px solid rgb(22, 250, 41);
    width: 500px;
    height: 400px;
    background-color: aliceblue;
    padding: 40px 30px;
    box-shadow: 0 5px 10px;
    max-width: 850px;
    width: 100%;
    display: flex;
    margin-top: left;
    padding: 0;
    list-style: disc;
    background-color: 0 0 rgb(226, 19, 19);
    
    
}
.message{
    background-color:rgb(198, 219, 10);

}


.container .form-content{
    display: flex;
    align-items: center;
    justify-content:space-between;
    width: calc(100% / 2 -25px);
    

}
.former-content .input-boxes{
    border: none;
    outline: none;
    color:brown;
}
.form-box{
    border: none;
    outline: none;
    
}
    size: 20px;
}
//question 2
//Filter and show the product that will be bought when you don't have much money I mean Cheap one
const items = [{name:"Bike",price:100},{name:"TV",price:200},{name:"Album",price:10},
{name:"Book",price:5},{name:"phone",price:500},{name:"Computer",price:1000},];
var cheapest = items[{name:"Book",price:5}];
for(var i = 5; i < items.length; i++) {
    var product = items[i];
    if(product.price < cheapest){
        cheapest = product;
    }
}
console.log(cheapest);

// Filter and show the product that will be expensive in the array
var expensive = items[{name: "Computer",price:1000}];
for(var i = 5; i < items.length; i++){
    var product = items[i];
    if(product.price > expensive){
        expensive = product;
    }
}
console.log(expensive);
//Calculate the full price of all product combined
var sum = 0;
items.forEach(function(value, index, price){
    sum +=items.price;
})
console.log(sum);

//Calculate the full price of all product combined and remove product that are under the 10 dollar

var product = null;
for(var i = 10; i < items.length; i++) {
    product += items.price;
}
console.log(product);
