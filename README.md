@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-family: 'Poppins', sans-serif;
}

html{
    font-size: 62.5%;
}

body{
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: black;
    color: white;
}

header{
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: transparent;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo{
    font-size: 3rem;
    color: #a3bce8;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;
}

.logo:hover{
    transform: scale(1.1);
}

nav a{
    font-size: 1.9rem;
    color: white;
    margin-left: 4rem;
    font-weight: 500;
    transition: 0.3s ease;
    border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active{
    color: #a3bce8;
    border-bottom: 3px solid #a3bce8;
}

@media(max-width:995px){
    nav{
        position: absolute;
        display: none;
        top: 0;
        right: 0;
        width: 40%;
        border-left: 3px solid #a3bce8;
        border-bottom: 3px solid #a3bce8;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: #161616;
        border-top: 0.1rem solid rgba(0,0,0,0.1);
    }

    nav.active{
        display: block;
    }

    nav a{
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
    }

    nav a:hover,
    nav a.active{
        padding: 1rem;
        border-radius: 0.5rem;
        border-bottom: 0.5rem solid #b74b4b;
    }
}

section{
    min-height: 100vh;
    padding: 5rem 9% 5rem;
}

.home{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8rem;
    background-color: black;
}

.home .home-content h1{
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
}

span{
    color: #a3bce8;
}

.home-content h3{
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.home-content p{
    font-size: 1.6rem;
}

.home-img{
    border-radius: 50%;
}

.home-img img{
    position: relative;
    width: 32vw;
    border-radius: 40%;
    box-shadow: 0 0 25px solid #a3bce8;
    cursor: pointer;
    transition: 0.2s linear;
}

.home-img img:hover{
    font-size: 1.8rem;
    font-weight: 500;
}

.social-icons a{
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid #a3bce8;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: #a3bce8;
}

.social-icons a:hover{
    color: black;
    transform: scale(1.3) translateY(-5px);
    background-color: #a3bce8;
    box-shadow: 0  0 25px #a3bce8;
}

.btn{
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: black;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: #a3bce8;
    letter-spacing: 0.3rem;
    font-weight: 600;
    border: 2px solid #a3bce8;
    transition: 0.3s ease;
    cursor: pointer;
}

.btn:hover{
    transform: scale3d(1.03);
    background-color: #a3bce8;
    color: black;
    box-shadow: 0 0 25px #a3bce8;
}

.typing-text{
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.typing-text span{
    position: relative;
}

.typing-text span::before{
    content: "software Developer";
    color: #a3bce8;
    animation: words 20s infinite;
}

.typing-text span::after{
    content: "";
    background-color: black;
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid black;
    right: -8;
    animation: cursor 0.6s infinite;
}

@keyframes cursor{
    to{
        border-left: 3px solid #a3bce8;
    }
}

@keyframes words{
    0%, 20%{
        content: "Web Developer";
    }
    21%, 40%{
        content: "Developer";
    }
    41%, 60%{
        content: "Web Designer";
    }
    61%, 80%{
        content: "Youtuber";
    }
    81%, 100%{
        content: "Script Writer";
    }
}

@media (max-width: 1000px){
    .home{
        gap: 4rem;
    }
}

@media(max-width:995px){
    .home{
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3{
        font-size: 2.5rem;
    }

    .home-content h1{
        font-size: 5rem;
    }

    .home-img img{
        width: 70vw;
        margin-top: 4rem;
    }
}

<!DOCTYPE html>
<html lang="en">
    
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <link rel="stylesheet" href="styl.css">
    <title>Portfolio Website</title>
</head>
<body>
    <header>
        <a href="#" class="logo">Rendy</a>

        <nav>
            <a href="#" class="active"> Home</a>
            <a href="#" >Services</a>
            <a href="#" >Skills</a>
            <a href="#" >Education</a>
            <a href="#" >Experience</a>
            <a href="#" >Contact</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="image/_Xiao-removebg-preview.png" alt="">
        </div>
        <div class="home-content">
            <h1>Hi, It's <span>Rendy</span></h1>
            <h3 class="typing-text">I'm a <span></span></h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minus labore dolores esse. Odit similique doloribus tenetur doloremque, sunt commodi in ipsa repudiandae debitis deleniti blanditiis quibusdam quaerat neque asperiores ea.</p>
            <div class="social-icons">
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-github"></i></a>
                <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
            </div>
            <a href="#" class="btn">Hire me</a>
        </div>
    </section>
</body>
</html>

- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
rl-rendy/rl-rendy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
