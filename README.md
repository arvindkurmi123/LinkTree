<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reserva</title>
    <!-- fonts -->

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link 
        href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
    <link
        href="https://fonts.googleapis.com/css2?family=Aboreto&display=swap" rel="stylesheet">


    <!-- styles -->

    <style>
        * {
            margin: 0;
            padding: 0;
        }
        .logo {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border-left-width: 68px;
            margin-left: 65px;
            padding-top: 10px;
            padding-bottom: 10px;
            /* padding-right: 10px; */
        }

        .text1 {
            color: white;
            position:fixed;
            padding: 30px;
        }
        .text2 {
            color: rgb(0, 0, 0);
            font-size: 44px;
            padding: 30px;
            padding-left: 170px;
            /* float: left; */
            font-family: 'Aboreto', cursive;
        }

        .background1 {
            background-image: url(background.jpg);
            background-attachment: fixed;
            background-size: cover;
            background-repeat: no-repeat;
            height: 100vh;
        }
        

        #first_image {
            float: left;
            width: 49%;
        }

        #second_image {
            float: right;
            width: 49%;
        }

        .white_bg {
            background-color: white;
        }

        .new_container {
            width: 1465px;
            border: 3px solid rgb(62, 60, 60);
            border-radius: 7px;
            background-color: rgba(255, 252, 156, 0.26);
            margin: 33px auto;
            padding: 5px 10px;
            margin: 18px 5px;
        }

        .quick-links{

            color: white;
            padding: 40px;
            font-size: 20px;
        }

        #h3headings{
            font-size: 40px;
            color: white;
            font-family: 'Aboreto', cursive;
        }
        #h2headings{
            font-size: 20px;
            color: rgb(255, 255, 255);
            float:left;
            width: 40%;
            padding-right:  30px;
            font-style: oblique;
        }
        #h1headings{
            font-size: 20px;
            padding-top: 10px;
            padding-right: 30px;
            padding-bottom: 10px;
            color: rgb(255, 255, 0);
            
            font-style:initial;
        }
        .lfloat{
            /* padding-top: 20px; */
            padding-left: 60px;
            float: left;
            /* width: 50%; */
        }
        .rfloat{
            padding-top: 80px;
            padding-left: 60px;
            float: right;
            width: 40%;
        }
        .image-sizing{
            /* padding: 20px;
            padding-bottom: 0px; */

            box-sizing: border-box;
        }
        .image-sizing .container{
            display: flex;
            overflow-x: scroll;
            padding: 24px;
            width: 300px;
            scroll-snap-type: x mandatory;
            scroll-padding: 24px;
            border-radius: 8px;
            gap: 12px;
        }
        .image-sizing .container .item{
            flex: 0 0 100%;
            padding: 24px;
            border-radius: 8px;
            scroll-snap-align: start;
        }
        .middle-class{
            font-size: 35px;
            /* clear: both; */
            margin: 20px auto;
            /* float: right; */
            width: 40%;
        }

        .welcome{
            text-align: center;
            font-size: 33px;
            color: aliceblue;
        }

        .testimonial{
             /* margin: 10px auto 10px; */
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            grid-gap: 20px;
        }

        .testimonial .card{
            position:relative;
            margin:0 auto;
            width: 350px;
            border-radius: 20%;
            /* background: rgb(97, 94, 94); */
            padding:20px;
            box-sizing: border-box;
            text-align: center;
            box-shadow: 0 20px 40px rgba(58,58,58,0.5);
            overflow: hidden;
        }

        .testimonial .card .layer{
            position:absolute;
            top:calc(100% - 2px);
            left:0;
            height: 100%;
            width: 100%;
            background: linear-gradient(#a7a7a7, #47585e  ,#4e4f4f);
            z-index: 1;
            transition: 1.5s;
        }

        .testimonial .card:hover .layer{
            top:0;
        }

        .testimonial .card .content{
            position: relative;
            z-index: 2;
            font-family: fantasy;
            border-radius: 50%;
        }

        .testimonial .card .content p{
            font-size: 18px;
            line-height: 24px;
        }

        .testimonial .card .content .image{
            width: 128px;
            height: 128px;
            margin: 0 auto;
            border-radius: 50%;
            overflow: hidden;
            display: inline;
            border: 4px solid rgb(226, 253, 21);
            box-shadow: 0 10px 20px rgb(151, 162, 30);
        }

        .testimonial .card .content .details h2{
            font-size: 18px;
            font-family: cursive;
            font-weight: bold;
            color: #0d2b39;
        }

        .testimonial .card .content .details span{
            color: #03a9f4;
            font-size: 20px;
            transition:2s;
            color: rgb(243, 255, 183);
        }

        .testimonial .card:hover .content .details span{
            color: rgb(1, 221, 255);
            font-family:fantasy;
        }


        ul{

            margin-top: 180px;
            padding: 0;
            display: flex;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 100%;
        }

        ul li{
            list-style: none;
            margin: 0 15px;
        }

        ul li a{
            position: relative;
            display: block;
            width: 100px;
            height: 100px;
            background: #333 ;
            text-align: center;
            line-height: 100px;
            border-radius: 50%;
            font-size: 30px;
            color: #666;
            transition: .1s;
        }
        ul li a::before{
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: #ffffff;
            transition : .5s;
            transform: scale(.9);
            z-index: -1;

        }

        ul li a:hover::before{
            transform: scale(1.1);
            box-shadow: 0 0 35px #ffffff;

        }

        ul li a:hover{
            color: #f7f7f7;
            box-shadow: 0 0 5px #ffee10;
            text-shadow:  0 0 5px #ffee10;
        }
    </style>


</head>
<body >
    <!-- first page start -->
    


    <div class="background1"  style="position: relative; min-height: 100%; top: 0px;">
     <!-- Top Bar Start -->
     <span>
     <img class="logo" src="ak.png" alt="Mylogo"></span>
      <span><strong class="text1" style="font-size: 34px;">Arvind Kurmi</strong>
     <span style="color: white;">23 Gourishankar ward Hatta, Damoh, Madhya Pradesh 470775</span>
    </span>

       <span><a href="forms.html" target="_blank" class="quick-links" style="float: right;">contact me</a></span>
       <span><a href="https://www.sgsits.ac.in/" target="_blank" class="quick-links" style="float: right;">Achievements</a></span>
    
    <!-- <span
         style="color:white ;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;23 Gourishankar ward Hatta, Damoh, Madhya Pradesh 470775
    </span> -->

        <br><br><hr style="color:rgb(254, 252, 252); background-color:rgb(252, 251, 251); height: 1px; border: none;">

   <br>
    <!-- MIDDLE HEADING -->
    <div class="welcome">&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp WELCOME TO THE HOME</div>
    <!-- Left side -->
    <div class="lfloat">
    <!-- <h3 id="h3headings">Welcome to the home!</h3> -->
    <div class="image-sizing">
    <!-- <img src="alexander2.jpg" alt="artist image" style="width: 542px;"> -->



    <!-- <div class="container">
        <div class="item">
            <h4>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</h4>
            <div>
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Tempora error delectus harum accusantium in ducimus nesciunt.
            </div>
        </div>
        <div class="item">
            <h4>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum!</h4>
            <div>
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Tempora error delectus harum accusantium in ducimus nesciunt.
            </div>
        </div>
        <div class="item">
            <h4>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</h4>
            <div>
                Lorem ipsum dolor, lorem10 sit amet consectetur adipisicing elit. Tempora error delectus harum accusantium in ducimus nesciunt.
            </div>
        </div>
    </div> -->



    <div class="testimonial">
        <div class="card">
            <div class="layer"></div>
            <div class="content">
                <br>
                <div class="image"><img style="border-radius: 50%; box-shadow: 0px 0px 16px white; height: 140px; width: 140px;" src="arvind.jpg" alt="photo">
                </div>
                <div class="details">
                    <BR></BR> <br> <span style="font-family:cursive;">Find the links below </span>
                </div>
            </div>
        </div>
    </div>

    
    </div>
    <br>
    <!-- <div class="app">
        <img  style="height: 100px; width: 100px; border-radius: 50%;" src="https://cdn4.iconfinder.com/data/icons/social-messaging-ui-color-shapes-2-free/128/social-twitter-square2-512.png" alt="Twitter logo">
    </div> -->
    
        
        

    </div>



    <!-- Right side -->
    <div class="rfloat">
    <h1 id="h1headings">"The true mark of a master is not in the skills they possess, but in their openness to acquire new ones. I am always eager to embrace the cutting edge of technology." </h1><br>
    <h2 id="h2headings">"The future belongs to those who understand new technologies and can harness them to create a better world."
    <br><br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Bill Gates</h2>
    <h2 id="h2headings">"I strive to be a bridge between technology and nature, connecting the two for a harmonious future."
        <br><br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Arvind Kurmi
    </h2>
    </div>

    

        <ul>
            <li>
                <a href="https://github.com/arvindkurmi123">
                    <img  style="height: 100px; width: 100px; border-radius: 50%;" src="git.png" alt="GitHub logo">

                </a>
            </li>
            <li>
                <a href="https://twitter.com/Arvind_kurmi_">
                    <img  style="height: 100px; width: 100px; border-radius: 50%;" src="twitter.jpg" alt="Twitter logo">
                    
                </a>
            </li>
            <li>
                <a href="https://www.linkedin.com/in/arvind-kurmi-940558230/">
                    <img style="height: 100px; width: 100px; border-radius: 50%;" src="linkedin.png" alt="LinkedIn logo">

                </a>
            </li>
            <li>
                <a href="https://www.instagram.com/photo.com08/">
                    <img style="height: 100px; width: 100px; border-radius: 50%;" src="instagram.png" alt="insta logo">
                </a>
            </li>
        </ul>

        <ul style="margin-top: 300px;">
            <li>
                <a href="https://web.telegram.org/k/#Arvind_kurmi">
                    <img  style="height: 100px; width: 100px; border-radius: 50%;" src="telegram.png" alt="GitHub logo">

                </a>
            </li>
            <li>
                <a href="https://www.facebook.com/arvindkurmi08/">
                    <img  style="height: 100px; width: 100px; border-radius: 50%;" src="facebook.png" alt="Twitter logo">
                    
                </a>
            </li>
            <li>
                <a href="https://www.youtube.com/channel/UCKbSq_MokkAlIx6s-FR3pFw">
                    <img style="height: 100px; width: 100px; border-radius: 50%;" src="youtube.png" alt="LinkedIn logo">

                </a>
            </li>
            <li>
                <a href="https://leetcode.com/arvind_kurmi_lc/">
                    <img style="height: 100px; width: 100px; border-radius: 50%;" src="leetcode2.png" alt="insta logo">
                </a>
            </li>
        </ul>

    </div>

<!-- first page end  -->

</body>
</html>
