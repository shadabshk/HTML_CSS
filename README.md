<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facebook - Login or Sign-Up</title>
    <link rel="icon" href="https://www.freepnglogos.com/uploads/facebook-logo-design-1.png">

</head>
<style>
    * {
        margin:0;
        padding:0;
        font-family:Arial, Helvetica, sans-serif;
        box-sizing: border-box;
    }   
    body {
        background-color: #f0f2f5;
        position: relative;
        height: 100vh;
        overflow-x: hidden;
    }
    #main_container{
        display:flex;
        

    }

    #recent_login{
        display: flex;
        flex-direction: column;
       
        position: relative;
        margin-left: 20vw;
        top:13vh;
        margin-right:5vw;
    }
    
    #recent_login > #facebook{
        height: 70px;
        width:198px;
        margin: -20px;
    }
    #recent_login > #title{
        font-size: 28px;
        font-weight: normal;
        line-height: 35px;
        margin-top: 20px;
        margin-bottom: 5px;
    }
    #recent_login > #subtitle{
        color:#606770;
        font-size: 15px ;
        line-height: 15px;
        margin-bottom: 20px;
        font-weight: 400;
    }
    #card{
        display:flex;
        flex-direction: row;
    }
    #card_1, #card_2{
        position: relative;
        background-color: white;
        margin-right: 10px;
        border-radius: 5px;
    }
    #card_1:hover, #card_2:hover{
        box-shadow:0 8px 16px 0 rgba(0,0,0,0.2);
        cursor:pointer;
        transition: box-shadow 0.3s;
    }
    #card_1_img,#card_2_img{
        height: 160px;
        width:160px;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
    }
    #add_account{
        color: #166fe1 s;
    }
    .username{
        font-size: 18px;
        line-height: 22px;
        padding: 12px;
        text-align: center;
        color: rgb(75,79,86);
    }
    #notifications{
        background-color: rgb(236,58,58);
        color:white;
        position: absolute;
        right:-5px;
        top:-5px;
        border-radius: 50%;
        height: 25px;
        width: 25px;
        text-align: center;
        font-size: 12px;
        line-height: 25px;;
    }
    #cancel{
        position: absolute;
        left: 8px;
        color: white;
        top:5px;
        border-radius: 50%;
        height: 20px;
        width:20px;
        background-color: rgb(63,62,62);
        opacity: 0.5;
    }

    #card_1:hover #cancel{
        background-color: white;
        opacity: 1;
        color:rgb(194,193,193);
        height: 25px;
        width:25px;
        line-height: 23px;
        font-size: 25px;
        transition: 0.3s;
        text-align: center;
    }
    #login{
        position: relative;
        background-color: #ffffff;
        height:350px;
        width: 300px;
        border-radius: 10px;
        display: flex;
        flex-direction: column;
        top:18vh;
        justify-items: center;
        padding:10px 10px 20px 10px;
        align-items: center;
        box-shadow: 0 5px 5px 3px gainsboro;
        margin-left: 120px;
    }
    #login > a{
        margin:18px 0;
        text-decoration: none;
        font-size: 15px;
        color: 1877f 2px;
    }
    #login > a:hover{
        text-decoration: underline;
        cursor: pointer;
    }   
    hr{
        width:95%;
        height:0.1%;
        background-color: rgb(194,193,193);
        border:none;
    } 
    #login > input[type=text], #login > input[type=password]{
        height:35px;
        margin:8px 0;
        border-radius: 5px;
        padding-left: 10px;
        width:95%;
        font-size: 16px;
        border:1.5px solid #EEEFF0;
    }
    #login > input[type=password]{
        margin-bottom: 10px;
    }
    #login > input[type=text]:focus, #login > input[type=password]:focus{
        outline:none;
        border:1px solid blue;
        box-shadow: 0 0 5px #719ece;
        caret-color: blue;
    }
    #login_button{
        background-color: #1877f2;
        color: #ffffff;
        font-size: 20px;
        border-radius: 5px;
        border:none;
        height:40px;
        width: 95%;
        font-weight: bold;
        margin-bottom: 10px;

    }
    #login_button:hover{
        background-color: #166;
        cursor: pointer;
    }
    #create_account{
        display: flex;
        justify-content: center;
        align-content: center;
       padding-left: 20px;
        background-color: #42b72a;
        color:white;
        font-size: 18px;
        width:80%;
        height:40px;
        border:none;
        border-radius: 5px;
        margin-top: 20px;
    }
    #create_account:hover{
        cursor: pointer;
        background-color: aquamarine;
    }
    footer {
        display:flex;
        background-color: #ffffff;
        position: absolute;
        bottom: 0;
        font-size: 12px;
        width:100vw;
        height:80px;
        justify-content: center;
        align-items: center;
    }
    table,td,th{
        border-collapse: collapse;
    }

    @media screen and (max-width: 1114px){
        #recent_login{
            left: 70px;
            margin-right: 22vw;
        }
        #login{
            right:30px;
        }
        }
    @media screen and (max-width:900px) {
        body{
            height: 150vh;
        }
        #container{
            flex-direction:column;
            align-items: center;
            justify-content: center;
        }   
        #recent_login{
            margin-right: 0;
            align-items: center;
            left: 0;
            top: 20px;

        }
        #card_1{
            margin-right: 5px;
        }
        #card_2{
            margin-left: 5px;
            margin-right: 0;
        }
        #login{
            text-align: center;
            left: 0;
            margin-right: 0;
            margin-top: -30px;
            top: 80px;
        }
        #recent_login,#login{
            position: relative;
        }
        #footer{
            position: absolute;
            padding:20px;
            width:100vw;
        }
        @media screen and (max-height:670px){
            footer{
                position: relative;
                top: 100px;
            }
        }
    }  
    
</style>
<body>
    <div id="main_container">
        <div id="recent_login">
            <img src="https://static.xx.fbcdn.net/rsrc.php/y8/r/dF5SId3UHWd.svg" alt="Facebook_Logo" id="facebook">
        <div id="title">Recent Logins </div>
        <div id="subtitle">Click your Picture or add an account</div>
        <div id="card">
            <div id="card_1">
                <div id="cancel">x</div>
                <div id="notifications">99+</div>
                <img id="card_1_img" src="https://bestprofilepictures.com/wp-content/uploads/2021/04/Cool-Profile-Picture-768x798.jpg" alt="you">
                <div class="username">Lingard</div>
            </div>
            <div id="card_2">
                <img id="card_2_img" src="https://icons-for-free.com/iconfiles/png/512/contact+add+friend+add+user+friend+request+icon-1320166636216988036.png" alt="Other Account">
                <div id="add_account" class="username">Add Account</div>
            </div>
        </div>
        </div>
        <div id="login">
            <input type="text" placeholder="Email or Phone Number">
            <input type="password" placeholder="Password">
            <input type="button" value="Log In" id="login_button">
            <a href="#">Forgot Password ?</a>
            <hr style="width:95% ;">
            <input type="=button" value="Create New Account" id="create_account">
        </div>
</div>

<footer> 
    <div>
       <table>
           <tr>
               <td>English</td>
               <td>Hindi</td>
               <td>Tamil</td>
           </tr>
           <tr>
               <td>Bengali</td>
               <td>Marathi</td>
               <td>Telugu</td>
           </tr>
       </table>
      
    </div>
</footer>  


</body>
</html>
