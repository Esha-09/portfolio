
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
            <h1>HI, I am <span>Esha</span> Mahara</h1>
           </div>
        </div>
</div>

<div id = "About">
    <div class="container">
        <div class = "row">
            <div class = about-col-1>
                <img src="user1.jpeg" alt="">
            </div>
            <div class = about-col-2>
                <h1 class="sub-title">About Me</h1>
                <p>Hello there! MY name is Esha Mahara. I am doing my bachelors of technology form graophic era bhimtal.
                    I have done my schooling form Beersheba senior secondary school haldwani.
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
                        <li><span>karan</span><br>A good student</li>
                        <li><span>karan</span><br>A good student</li>
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
                <h2>karan</h2>
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
                <img src="work1.jpeg" >
                <div class = "layer">
                    <h3>KARAN</h3>
                    <p>This is karan </p>
                    <a href="#"><i class="fa-solid fa-trophy"></i></a> 
                </div>
            </div>
            <div class = work>
                <img src="work1.jpeg" >
            </div>
            <div class = work>
                <img src="work1.jpeg" >
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
                <h1 class = sub-title> Contact Me</h1>
                <p><i class="fa-regular fa-envelope"></i> karann.bhanwal@gmail.com</p>
                <p><i class="fa-solid fa-phone"></i>7452009499</p>
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
        <p><i class="fa-solid fa-heart"></i>copyright @karan</p>
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
</html>
# portfolio
