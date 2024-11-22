<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA_Compatible" content = "IE=edge">
    <title>Personal Portfolio</title>
    <link rel="stylesheet" href="style.css">;
    <script src="https://kit.fontawesome.com/743bc8534e.js" crossorigin="anonymous"></script>
</head>
<body>
    <div id = "header">
        <div class="container">
            <nav>
                <img src = "logo.png" class = "logo">
                <ul  id = "sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#About">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#Portfolio">Portfolio</a></li>
                    <li><a href="#Contact">Contact</a></li>
                    <i class="fa-solid fa-x" onclick="closemenu()" ></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i> 
            </nav>
           <div class = "header-text">
            <p>Btech Student</p>
            <h1>HI, We ara <span> Esha</span> Mahara<span></h1>
           </div>
        </div>
</div>

<div id = "About">
    <div class="container">
        <div class = "row">
            <div class = about-col-1>
                <img src="imeges/US.JPG.jpg" alt="">
            </div>
            <div class = about-col-2>
                <h1 class="sub-title">About US</h1>
                <p>Hello there! I am  Esha Mahara .  I am persuing Bachelors of technology form graophic era bhimtal.
                    
                </p>
                <div class = "tab-titles">
                    <p class = "tab-links active-link" onclick="opentab('Skills')">Skills</p>
                    <p class = "tab-links" onclick="opentab('Experience')">Experience</p>
                    <p class = "tab-links" onclick="opentab('Education')">Education</p>
                </div>
                <div class="tab-contents active-tab" id = "Skills">
                    <ul>
                        <li><span>Btech</span><br>A good student</li>
                        <li><span>Btech</span><br>A good student</li>
                        <li><span>Btech</span><br>A good student</li>
                    </ul>
                </div>
                <div class="tab-contents" id="Experience" >
                    <ul>
                        <li><span>hello</span><br>A good student</li>
                        <li><span>hello</span><br>A good student</li>
                        <li><span>Btech</span><br>A good student</li>
                    </ul>
                </div>
                <div class="tab-contents" id = "Education">
                    <ul>
                        <li><span>Esha</span><br>A good student</li>
                        <li><span>Harshita</span><br>A good student</li>
                        <li><span>Btech</span><br>A good student</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>

<div id = "services">
    <div class = "container">
        <h1 class = "sub-title">Our Services</h1>
        <div class="services-list">
            <div>
                <h2>Web Design</h2>
                <p>kdjvnedjsvnsjvnoejfvnojnv vvj o v vrieo rno veovn eo</p>
                <a href="#">Learn more</a>
            </div>
            <div>
                <h2>hello</h2>
                <p>kdjvnedjsvnsjvnoejfvnojnv vvj o v vrieo rno veovn eo</p>
                <a href="#">Learn more</a>
            </div>
            <div>
                <h2>Esha</h2>
                <p>kdjvnedjsvnsjvnoejfvnojnv vvj o v vrieo rno veovn eo</p>
                <a href="#">Learn more</a>
            </div>
        </div>
    </div>
</div>
<div id = "Portfolio">
    <div class = "container">
        <h1 class = "sub-title">Our Work</h1>
        <div class="work-list">
            <div class = work>
                <img src="imeges/OURWORK.jpg" >
                <div class = "layer">
                    <h3>Esha</h3>
                    <p>This is our work </p>
                    <a href="#"><i class="fa-solid fa-trophy"></i></a> 
                </div>
            </div>
            <div class = work>
                <img src="imeges/OUR WORK.JPG.jpg" >
            </div>
            <div class = work>
                <img src="imeges/OUR WORK.jpg" >
            </div>
        </div>
            <a href="#" class = btn>See more</a>
    </div>
</div>
<div id = "Contact">
    <div class = "container">
        <h1 class = "row"></h1>
        <div class="row">
            <div class = contact-left>
                <h1 class = sub-title> Contact us</h1>
                <p><i class="fa-regular fa-envelope"></i> maharaesha@gmail.com</p>
                <p><i class="fa-solid fa-phone"></i>6397289430</p>
                <div class="social-icons">
                    <a href=""><i class="fa-brands fa-instagram"></i></a>
                    <a href=""><i class="fa-brands fa-x-twitter"></i></a>
                    <a href=""><i class="fa-brands fa-facebook"></i></a>
                </div>
                <a href="download.pdf" download class="btn btn2 ">Download</a>
            </div>
            <div class = contact-right>
                <form >
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name = "Name" placeholder="Your email" required >
                    <textarea name="Message" row = "6" placeholder="Your message"></textarea>
                    <button type ="submit" class="btn btn2"> Submit</button>
                </form>
            </div>
    </div>
    <div class="copyright">
        <p><i class="fa-solid fa-heart"></i>copyright @esha</p>
    </div>
</div>


<script>
    var tablinks= document.getElementsByClassName("tab-links");
    var tabcontents= document.getElementsByClassName("tab-contents");

    function opentab(tabname){
        for(tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for(tabcontent of tabcontents){
            tabcontent.classList.remove("active-tab");
        }
        event.currentTarget.classList.add("active-link");
        document.getElementById(tabname).classList.add("active-tab");
    }
</script>
<script>
    var sidemeu= document.getElementById("sidemenu");
    function openmenu(){
        sidemeu.style.right = "0";
    }
    function closemenu(){
        sidemeu.style.right = "-200px";
    }
</script>
</body>
</html>![US JPG](https://github.com/Esha-09/portfolio/assets/145591365/5eb2bd4e-e444-4656-9ec6-30bacc1240a9)
![OURWORK](https://github.com/Esha-09/portfolio/assets/145591365/4406613d-418f-4313-8907-2badd1b171ea)
![OUR WORK JPG](https://github.com/Esha-09/portfolio/assets/145591365/5339556e-8767-4c50-80af-68f227598917)
![OUR WORK](https://github.com/Esha-09/portfolio/assets/145591365/200e568d-ace8-4e68-8f6e-5d04e0cf197b)
