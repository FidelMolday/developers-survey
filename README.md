developers survey
<!DOCTYPE HTML>
<html>
 <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <meta http-equiv="x-UA-Compatible" content="ie=edge">
    <title>Survey Page</title>
 </head>
 <body>
  <header>
    <h1>Developers Survey</h1>
    <p>Give some information about you.</p>
  </header>
  <div class="survey">
    <div class="q1">
        <h3>What progrmming language do you learn?</h3>
        <ul class="option1">
            <li>Python</li>
            <li>Java</li>
            <li>C#</li>
            <li>Javascript</li>
        </ul>
    </div>
    <div class="q2">
        <h3>How  long have been coding?</h3>
        <ul class="option2">
            <li>Just started</li>
            <li>3-6 months</li>
            <li>6-12 months</li>
            <li>1-2 years</li>
        </ul>
    </div>
    <div class="q3">
        <h3>What`s your idea after learning coding?</h3>
        <ul class="option3">
            <li>Full time job</li>
            <li>Free lancing</li>
            <li>Side hustling</li>
            <li>No idea</li>
        </ul>
    </div>
  </div>
  <div class="end">
    <h1>Thank You</h1>
    <p>We will get back to you as soon as possible</p>
    <a href="index.html">Home</a>
  </div>
  <style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    body{
        font-family: "monserrat",sans-serif;
        text-align: center;
    }
    a{
        text-decoration: none;
        list-style: none;
    }
    li{
        text-decoration: none;
        list-style: none;
    }
    header{
        background: rgba(0,255,128);
        color: rgb(61,61,61);
        padding: 10px;
    }
    header p{
        font-size: 16px;
    }
    .survey{
        width: 80%;
        margin: 20px auto;
        background: royalblue;
        color: white;
        height: 200px;
        border-radius: 3px;
        box-shadow: 1px 1px 7px rgba(0,0,0,0.4);
    }
    .survey h3{
        margin: 8px;
        padding-top: 10px;
    }
    .survey li{
        margin: 10px;
        cursor: pointer;
    }
    .survey li:hover{
        background: cornflowerblue;
        width: 150px;
        margin: 0 auto;
        padding: 4px;
        border-radius: 3px;
        transition: 0.3s ease;
    }
    .end{
        background: royalblue;
        color: white;
        width: 80%;
        margin: 35% auto;
        padding: 20px 0;
        border-radius: 3px;
        box-shadow: 1px 1px 7px rgba(0,0,0,0.4);
    }
    .end h1{
        margin: 5px;
    }
    .end p{
        padding: 10px;
    }
    .end a {
        display: inline-block;
        margin-top: 10px;
        padding: 5px;
        border-radius: 4px;
        background: rgb(61,61,61);
        outline: none;
    }
    .end a:hover{
        box-shadow: 1px 1px 7px rgba(0,0,0,0.404);
        transition: 0.3s;
    }
    .q1{
        display: block;
    }
    .q2{
        display: none;
    }
    .q3{
        display: none;
    }
    .end{
        display: none;
    }
  </style>
  <script>
    const ul_1 = document.querySelector(".option1");
    const ul_2 = document.querySelector(".option2");
    const ul_3 = document.querySelector(".option3");

    const q1 = document.querySelector(".q1");
    const q2 = document.querySelector(".q2");
    const q3 = document.querySelector(".q3");

    const survey = document.querySelector(".survey");
    const end = document.querySelector(".end");
    
    //first question
    ul_1.addEventListener("click",function(){
        q1.style.display = "none";
        q2.style.display = "block";
    });

    //second question
    ul_2.addEventListener("click",function(){
        q2.style.display = "none";
        q3.style.display = "block";
    });

    //display thanks message
    ul_3.addEventListener('click',function(){
        q3.style.display = "none";
        survey.style.display = "none";
        end.style.display = "block";
    });
    </script>
 </body>
</html>
