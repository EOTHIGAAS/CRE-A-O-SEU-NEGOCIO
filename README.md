@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;1,100;1,300;1,400&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto',sans-serif;
}
body{
    background-color: #e3f0ff;
    min-height: 100vh;
}

.container{
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 4%;
}
nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}
nav .menu-icon{
    cursor: pointer;
    display: none;
}
nav .logo{
    font-size: 30px;
    font-weight: bold;
    color: #5654b3;
    text-decoration: none;
}
nav ul{
    display: flex;
    list-style:none;
    align-items: center;
}
nav ul li{
    padding: 0 15px;
    font-weight: bold
}
nav ul li a{
    text-decoration: none;
    font-size: 17px;
    text-transform: uppercase;
    color: #5654b3;
}
nav ul button{
    border: none;
    background-color: #5654b3;
    color: white;
    padding: 10px 20px;
    border-radius: 5px;
    font-size: 16px;
    letter-spacing: 1px;
    margin-left: 20px;
    cursor: pointer;
}
main{
    margin-top: 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.text-bx{
    width: 40%;
}
.text-bx h1{
    font-size: 3rem;
    text-transform: uppercase;
}
.text-bx h1 b{
    color: #f1676d;
    
}
.text-bx p{
    color: #000;
    font-weight: 400;
    margin-top: 20px;
    font-weight:bolder;
}
.text-bx .input-bx{
    margin: 20px 0;
    display: flex;
}
.text-bx .input-bx input{
    width: 60%;
    display: block;
    height: 50px;
    padding: 10px;
    border: none;
    outline: none;
    color: #8997b9;
    font-size: 16px;
}
.text-bx .input-bx input::placeholder{
    color: #8997b9;
}
.text-bx .input-bx button{
    outline: none;
    border: none;
    padding: 10px 20px;
    background-color: #5654b3;
    color: white;
    cursor: pointer;
    font-size: 15px;
}
.medias-socias{
    margin-top: 30px;
}

.medias-socias a{
    text-decoration: none;
}
.medias-socias i{
    font-size: 23px;
    margin: 0 3px;
    color: white;
    background-color: #372c62;
    padding: 7px;
    border-radius: 5px;
}
.img-bx{
    width: 40%;
}
.img-bx img{  
   width: 100%;
}
@media(max-width:970px){
    nav .menu-icon{
        display: block;
    }
    nav ul{
        position: fixed;
        width: 60%;
        height: 100%;
        top: 0;
        left: 0;
        transform: translateX(-100%);
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: baseline;
        transition: 0.3s ease-in;
        background-color: #5654b3;
    }
    nav ul.active{
        transform:translateX(0)
    }
    nav ul li{
        padding: 10px;
    }
    nav ul li a{
        font-size: 18px;
        color: white;
    }
    nav ul button{
        background-color: #f1676d;
        font-size: 18px;
        margin: 10px;
    }
    main{
        flex-direction: column;
    }
    .text-bx ,
    .img-bx{
        width: 100%;
        text-align: center;
    }
    .text-bx{
        margin-bottom: 40px;
    }
    .text-bx .input-bx{
        justify-content: center;
    }
}
