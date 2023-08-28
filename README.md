# ui-imageslider

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Slider</title>
    <link rel="stylesheet" href="../css/mystyle.css">
</head>
<body>
    <div class="container">
          <div class="wrapper">
              <div class="wrapper-holder">
                  <div id="slider-img-1"></div>
                  <div id="slider-img-2"></div>
                  <div id="slider-img-3"></div>
                  <div id="slider-img-4"></div>

              </div>
          </div>
          <div class="button-holder">
                <a href="#slider-img-1" class="button"></a>
                <a href="#slider-img-2" class="button"></a>
                <a href="#slider-img-3" class="button"></a>
                <a href="#slider-img-4" class="button"></a>
          
          
           </div>


      </div>
</body>
</html>

```
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  background-image: url(../images/white.jpg);
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  
}
.container{
  position: relative;
}
.container .wrapper{
width: 60vw;
height: 75vh;
box-shadow: 10px 10px 20px rgba(0,0,0,0.6);
margin:5rem auto;
overflow: hidden;
}

.container .wrapper-holder{
  display: grid;
  grid-template-columns: repeat(4,100%);
  height: 100%;
  width: 100%;
  animation: slider 30s ease-in-out infinite alternate;
}

.container #slider-img-1{
  background-image: url(../images/1.jpg);
  background-position: center;
}

.container #slider-img-2{
  background-image: url(../images/2.jpg);
  background-position: center;
}
.container #slider-img-3{
  background-image: url(../images/3.jpg);
  background-position: center;
}
.container #slider-img-4{
  background-image: url(../images/4.jpg);
  background-position: center;
}

.container .button-holder .button{
  background-color: rgb(248, 245, 245);
  width:15px;
  height: 15px;
  border-radius: 15px;
  display: inline-block;
  margin:.3rem;
}

.container .button-holder{
  position: absolute;
  left:45%;
  bottom:0%;
}
.button:hover{
  background-color:palegoldenrod;
}
@keyframes slider {
  0%{transform:translateX(0%);}
  10%{transform:translateX(0%);}
  20%{transform:translateX(-200%);}
  30%{transform:translateX(-200%);}
  40%{transform:translateX(-300%);}
  50%{transform:translateX(-300%);}
  60%{transform:translateX(-300%);}
  70%{transform:translateX(-300%);}
  80%{transform:translateX(-300%);}
  90%{transform:translateX(0%);}
  100%{transform: translateX(0%);}
  
}

```

```
