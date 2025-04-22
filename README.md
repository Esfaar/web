<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated </title>
    <!-- <link rel="stylesheet" href="style.css" type="text/css"> -->
    <style type="text/css">

*{
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
    box-sizing: border-box;
}

.banner{
    width: 100%;
    height: 100vh;
    background-color: rgb(245, 246, 247);
    padding: 30px 8%;
}

.navbar{
    width: 100%;
    display:flex;
    align-items: center;
    justify-content: space-between;
}

.navbar h1{

    color: #000;
    font-size: 30px;
    font-weight: 900;
}

.navbar h1:hover{
    color: blue;
    transform: scale(2);
}

nav ul li{
    
    list-style: none;
    display: inline-block;
    margin: 0 80px;

}

nav ul li a {
    text-decoration: none;
    color: #000;
    font-size: 15px;
    position: relative;
    z-index: 1;
    padding: 5px;
}

nav ul li a::before {
    content: "";
    width: 100%;
    height: 0px;
    background: rgb(42, 250, 181);
    left: 0;
    bottom: -5px;
    position: absolute;
    z-index: -1;
    border-bottom-left-radius: 8px;
    border-bottom-right-radius: 8px;
    transition: 0.5s ease;

}

nav ul li a:hover::before{
    height: 85px;

}

.btn{
    padding: 15px 10px;
    border: .5px solid rgb(42, 250, 181);
    border-radius: 4px;
    background: transparent;
    color: #000;
    position: relative;
    z-index: 1;
    cursor: pointer;
    transition: 1s;
   
}

/* span{
    width: 100%;
    height: 100%;
    background: rgb(42, 250, 181);
    top: 0;
    left: 0;
    position: absolute;
    z-index: -1;
} */

.btn:hover{
    background:  rgb(42, 250, 181);
    
}



.content
{
    margin-top: 50px;
   
}
.row{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    text-align: center;
}

.col-1{
    flex-basis: 50%;
    text-align: left;
}

.col-1 h1{
    font-size: 60px;
}

.col-1 p{
    font-size: 15px;
    line-height: 18px;
    margin: 20px 0px;
    color: rgb(42, 250, 181);

}

.col-2{
    flex-basis: 50%;
    margin-top: 70px;
}

.col-2 img{
    width: 300px;
    height: 300px;
    border-radius: 10px;
    margin: 10px;
    flex-wrap: wrap;
    transition: 0.5s;
    cursor: pointer;
}

.col-2 img:hover{

    transform: translateY(-10px);
}

.content-btn a{
    width: 140px;
    padding: 15px;
    border: .5px solid rgb(42, 250, 181);
    text-decoration: none;
    color: #000;
    margin-right: 10px;
    background-color: rgb(42, 250, 181);
    border-radius: 4px;
    transition: 0.5s ease;
    display: inline-block;
    text-align: center;

}

.content-btn a:hover{
    transform: scale(1.1);
}

    </style>
</head>
<body>

    <div class="banner">
    <div class="navbar">
    <h1>Logo</h1>
    <nav>
        <ul>
            <li><a href="#">HOME</a></li>
            <li><a href="#">ABOUT</a></li>
            <li><a href="#">CONTACT</a></li>
        </ul>
    </nav>
    <button type="button" class="btn">Contact Me</button>
</div>
<div>
    <div class="content">
        <div class="row">
            <div class="col-1"> <h1>My First Demo<br>Animated Menu</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur, fugiat maxime. Nostrum tempore</p>
        <div class="content-btn">
            <a href="#">Watch Video</a>
            <a href="#">Learn More </a>
        </div>
        </div>
            <div class="col-2">
                <img class="pic" src="images/desert.jpg">
                <img class="pic" src="images/ocean.jpg">
                <img class="pic"  src="images/ground.jpg">
                <img class="pic"  src="images/rock.jpg">
            </div>
        </div>
        </div>
    </div>
    
    
    
</body>
</html>
