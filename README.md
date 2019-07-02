# clone_pikalog

<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>KIPALOG</title>
    <link href="https://fonts.googleapis.com/css?family=Lato|Open+Sans|Oswald&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Roboto&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css" />
    <style type="text/css">
        *{
            margin: 0;
            padding: 0;
            border: 0;
            text-decoration: none;
            box-sizing: border-box;
        }

        html{
            background-color: #f7f5f3;
        }

        .clearfix{
            content: ' ';
            display: table;
            clear: both;
        }

        .a{
            color: white;
        }

        div#menu {
            max-width: 100%;
            max-height: 100%;
            text-align: center;
        }
        /*HEADER*/
        div#header{
            display: block;
            width: 100%;
            height: 50px;
            border: 1px solid black;
            background-color: #2c4762;
        }

        div#header a.logo{
            float: left;
            margin-left: 60px;
            height: 50px;
            line-height: 50px;
        }

        div#header a.register{
            float: right;
            margin: 9px 82px 9px 0px;
            width: 85px;
            height: 30px;
            line-height: 30px;
            border: 1px solid #6c7f91;
        }

        div#header a.register:hover{
            border: 1px solid #5a6a79;
        }
        /*HOME_PAGE*/
        #home_page{
            background-color: #f7f5f3;
            display: block;
        }
        /*ROW*/
        div#menu .row{
            padding-top: 70px;
        }

        div#menu .row h1{
            font-family: 'Oswald', sans-serif;
            font-size: 3em; /*1em=16px*/
            margin-bottom: 20px;;
            color: #00b5ad;
            text-align: center
        }

        div#menu .row p{
            font-family: 'Open Sans', sans-serif;
            font-size: 1em;
            text-align: center;
        }
        /*LOGIN*/
        div#menu .login{
            padding-top: 50px;
            display: block;
        }

        div#menu .login .email,
        div#menu .login .password{
            display: inline-block;
            margin: 1px -68px 20px 1px;
            width: 33%;
            height: 30px;
            border: 1px solid #d7d6d6;
            background-color: #ffffff;
        }

        div#menu .login .email #email,
        div#menu .login .password #password{
            width: 90%;
            font-family: 'Roboto', sans-serif;
            height: 100%;

        }

        /*SIGN*/
        div#menu .login .sign #btn{
            width: 33%;
            height: 30px;
            margin: 0px -68px 20px 0px;
            background-color: #59b96f;
            color: #ffffff;
            border-radius: 4px;
        }

        div#menu .login .sign #btn:hover{
            background-color: #53a967;
        }
        /*FORGOT PASSWORD*/
        div#menu .login #forgot_the_password{
            display: inline-block;
            font-family: 'Lato', sans-serif;
            width: 33%;
            height: 20px;
            margin: 0px -68px 0px 0px;
          /*border: 1px solid black;*/
        }

        div#menu .login #forgot_the_password p a{
                color: #00bbc6;
    height: 20px;
    line-height: 20px;
    float: left;
        } 
        /*BULKHEAD*/
        div#menu .bulkhead{
            width: 33%;
            height: 50px;
            margin: 0px -68px 20px 0px;
            display: inline-block;
            background-color: #f7f5f3;
        }
        /*BUILKHEAD1*/
        div#menu .bulkhead #bulk1{
            width: 40%;
            display: inline-block;
            margin: 0px 0px 25px -172px;
            border: 1px solid #d7d6d6;
        }
        /*BUILKHEAD2*/
        div#menu .bulkhead #bulk2{
            display: inherit;
            width: 30px;
            height: 30px;
            border-radius: 15px;
            margin: 10px;
            border: 1px solid #d7d6d6;
        }

        div#menu .bulkhead #bulk2 nav{
            width: 7px;
            height: 7px;
            border-top: 1px solid;
            border-right: 1px solid black;
            margin: 8px 0px 0px 10px;
            transform: rotate(133deg);
        }
        /*BUILKHEAD3*/
        div#menu .bulkhead #bulk3{
            width: 40%;
            display: inline-block;
            margin: 0px -172px 25px 0px;
            border: 1px solid #d7d6d6;
        }
        /*SHARE*/
        div#menu .share a{
            display: inline-block;
            width: 160px;
            height: 40px;
            line-height: 40px;
            list-style: none;
        }

        div#menu .share a{
            font-family: 'Roboto', sans-serif;
            color: #ffffff;
        }

        div#menu .share a.facebook{
            background-color: #2a5297;
        }

        div#menu .share a.facebook:hover{
            background-color: #284e90;
        }

        div#menu .share a.twitter{
            background-color: #00aced;
        }

        div#menu .share a.twitter:hover{
            background-color:#009ad4; 
        }

        div#menu .share a.github{
            background-color: #000000;    
        }

        div#menu .share a.github:hover{
            background-color: #2d2d2d;
        }

        div#menu .share a input{
            text-indent: -10000000px;
            width: 20px;
            height: 20px;
        }

        div#menu .share a:first-child{
            background-color: #2a5297;
        }

        div#menu .share a:nth-child(2){
            background-color: #3f90ca;
        }

        div#menu .share a:nth-child(3){
            background-color: #000000;
        }

        div#menu .share a input.facebook{
            background-image: url(https://banner2.kisspng.com/20171216/213/facebook-logo-png-5a35528eaa4f08.7998622015134439826976.jpg);
            background-repeat: no-repeat;
            background-size: 66px;
            background-position: center;
        }

        div#menu .share a input.twitter{
            background-image: url(https://cdn2.iconfinder.com/data/icons/social-media-square-set/960/Twitter_Sq-512.png);
            background-repeat: no-repeat;
            background-size: 54px;
            background-position: center;
            margin-right: 8px;
        }

        div#menu .share a input.github{
            background-image: url(https://image.flaticon.com/icons/svg/23/23957.svg);
            background-repeat: no-repeat;
            background-size: 28px;
            background-position: center;
            margin-right: 8px;
        }
    </style>
</head>
<body>
    <div id="menu">
        <!-- HEADER -->
        <div id="header">
            <!-- LOGO -->
            <a class ="logo a" href="#">KIPALOG</a>
            <!-- REGISTER -->
            <a class="register a"  href="#"><i class="fas fa-chalkboard-teacher"></i>Đăng ký</a>
        </div>
        <div id="home_page">
        <!-- ROW -->
        <div class="row">
            <h1>Kipalog</h1>
            <p>Chia sẻ và học hỏi kiến thức một cách dễ dàng hơn</p>
        </div>
        <div class="login">
            <!-- EMAIL -->
            <div class="email">
                <input id="email" type="email" placeholder="Email" autofocus="autofocus">
            </div>
            <div class="clearfix"></div>
            <!-- PASSWORD -->
            <div class="password">
                <input id="password" type="password" placeholder="Password" autofocus="autofocus">
            </div>
            <!-- SIGN -->
            <div class="sign">
                <!-- BTN -->
                <button type="submit" id="btn"><a herf="#">ĐĂNG NHẬP</a></button>
            </div>
            <!-- FORGOT THE PASSWORD -->
            <div id="forgot_the_password">
                <p><a href="">Quên password ?</a></p>
            </div>
        </div>
        </div>
        <!-- VÁCH NGĂN -->
        <div class="bulkhead">
            <div id="bulk1"></div>
            <div id="bulk2">
                <nav></nav>
            </div>
            <div id="bulk3"></div>
        </div>
        <!-- SHARE -->
        <div class="share">
            <ul>
                <a class="facebook" href="#"><input class ="facebook" type="submit" value="go">FACEBOOK</a>

<!-- Cách 2 -->
                <!-- <a href="#"><i class="fab fa-facebook"></i>FACEBOOK</a> -->
                <a class="twitter" href="#"><input class ="twitter" type="submit" value="go">TWITTER</a>

<!-- Cách 2 -->
                <!-- <a href="#"><i class="fab fa-twitter"></i>TWITTER</a> -->
                <a class="github" href="#"><input class ="github" type="submit" value="go">GITHUB</a>

<!-- Cách 2 -->
                <!-- <a href="#"><i class="fab fa-github"></i>GITHUB</a> -->
        </div>
    </div>
</body>
</html>
