<template>
  <div id="app">
    <Header/>
    <Powerful/>
    <Active/>
    <Services/>
    <Instructions/>
    <Contractors/>
    <Client/>
    <Question/>
    <Join/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Powerful from './components/Powerful.vue'
import Active from "./components/Active"
import Services from "./components/Services"
import Instructions from "./components/Instructions"
import Contractors from "./components/Contractors"
import Client from "./components/Client"
import Question from "./components/Question"
import Join from "./components/Join"
import Footer from "./components/Footer"


export default {
  name: 'App',
  components: {
    Header, Powerful , Active , Services , Instructions , Contractors, Client , Question,
    Join, Footer
  },
  mounted() {
    let onTopBtn = document.getElementById("scroll-btn")
    onTopBtn.onclick = () => {
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  }
}
</script>

<style>
body {
  font-family: 'Poppins', sans-serif;
}
@font-face {
	font-family: 'proxima_nova_rgregular';
	src: url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.eot');
	src: url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.eot?#iefix') format('embedded-opentype'), url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.woff') format('woff'),url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.ttf') format('truetype'),url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.svg#proxima_nova_rgregular') format('svg');
	font-weight: normal;
	font-style: normal;
}
@font-face {
	font-family: 'proxima_nova_rgbold';
	src: url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.eot');
	src: url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.eot?#iefix') format('embedded-opentype'),url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.woff') format('woff'),url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.ttf') format('truetype'),url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.svg#proxima_nova_rgbold') format('svg');
	font-weight: normal;
	font-style: normal;
}

@font-face {
	font-family: 'adelle_rgregular';
	src: url('https://litmus.com/fonts/Emails/adelle_reg-webfont.eot');
	src: url('https://litmus.com/fonts/Emails/adelle_reg-webfont.eot?#iefix') format('embedded-opentype'),url('https://litmus.com/fonts/Emails/adelle_reg-webfont.woff') format('woff'),url('https://litmus.com/fonts/Emails/adelle_reg-webfont.ttf') format('truetype'),url('https://litmus.com/fonts/Emails/adelle_reg-webfont.svg#adelle_rgregular') format('svg');
	font-weight: normal;
	font-style: normal;
}
.logo{
font-size: 30px;
height: 70px;
line-height: 70px;
}
.menu-item{
font-size: 18px;
list-style: none;
text-align: center;
width: 20%;
}
.menu-item a{
  font-family: 'proxima_nova_rgregular', Helvetica, Arial, sans-serif;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
    letter-spacing: normal;
  color: #757575;
  text-decoration: none;
  transition: 0.3s;

}
.menu-item a:hover{
  color: #8c9aa3;
  transition: 0.3s;
}
.menu{
  margin-top: 30px;
display: flex;
flex-direction: row;
justify-content: space-around;
flex-wrap: wrap;
padding-left: 50px;
z-index: 300;
float: right;
}
.container-fluid{
padding-right: 30px;
padding-left: 30px
}
.banner-image{
z-index: 200;
}
.banner-image img{
max-width: 100%;
max-height: 100%;

}
.banner-text{
max-width: 60%;
background-color: #eef3fa;
z-index: 100;
height: 0;
padding-bottom: 45%;
position: absolute;
top: 0;
right: 0;
}
.banner-content{
  max-width: 60%;
  margin: 20% auto;
  padding-left: 10%;
}
.banner-content h1{
  font-family: 'Poppins', sans-serif;
  font-weight: 300;
  font-size: 3.5vw;
}
.banner-content p{
font-size: 16px;
color: #757575;
}
.banner-content button{
margin-top: 10px;
background-color: #77c977;
text-align: center;
color: #ffffff;
font-size: 18px;
width: 205px;
height: 60px;
box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);
border: none;
transition: 0.3s;
}
.banner-content button:hover{
  transition: 0.3s;
  background-color: white;
  border: 2px solid #77c977;
  color: #77c977;
}
.banner-content i{
padding-left: 10px;
}
.banner-dots{
width: 300px;
height: 300px;
margin : -150px auto;

}
.banner-dots img{
max-height: 300px;
max-width: 300px;
}
.powerful-header{
margin-top: 200px;
}
.powerful-header h1{
margin: 0 auto;
margin-top: 50px;
position: relative;
padding-bottom: 10px;
text-align: center;
font-family: 'Poppins', sans-serif;
font-size : 45px;
font-weight: 400;
color: #254266;
width: 100%;

}
.powerful-header h1:after{
content: "";
background: #77c977;
position: absolute;
left: 49%;
bottom: 0;
width : 2%;
height: 2px;
}
.powerful-header p{
font-size: 17px;
color: #757575;
line-height: 33px;
letter-spacing: 0.51px;
margin: 0 auto;
width: 680px;
padding-top: 5px;
text-align: center;
}
.powerful-banner{
  display: inline-block;
  position: relative;
  z-index: 500;
}
.powerful-banner img{
max-width: 100%;
position: relative;
}
.powerful-number{
position: absolute;
z-index: 200;
width: 20px;
height: 20px;
border-radius: 20px;
font-size: 14px;
}
.num-1{
background: #77c977;
color: white;
line-height: 20px;
text-align: center;
left: 18%;
margin-top: -8%;
}
.num-2{
background: #ffc212;
color: white;
line-height: 20px;
text-align: center;
left: 32%;
margin-top: -28%;
}
.num-3{
background: #5e0cef;
color: white;
line-height: 20px;
text-align: center;
right: 34.5%;
margin-top: -11%;
z-index: 400;
}
.powerful-chat{
  position: absolute;
  z-index: 1000;
  right: 25%;
  bottom:28%;
}
.powerful-chat1{
  margin-bottom: 10px;
}
.powerful-chat1 img{
float: left;
max-width: 100%;
max-height: 100%;
}
.powerful-chat2 img{
float: left;
max-width: 100%;
max-height: 100%;
}
.chat-1{
padding-left: 18px;
padding-right: 10px;
margin-left: 55px;
width: 254px;
height: 120px;
background-color: white;
border-radius: 10px;
padding-top: 15px;
}
.chat-1 p{
color: #1c2e40;
font-size: 15px;
float: left;
line-height: 23px;
letter-spacing: normal;
}
.chat-1 h5{
font-size: 14px;
color: #8c9aa3;
}
.chat-1 img{
max-width: 15px;
float: none !important;
max-height: 16px;
}
.arrow-down {
width: 0;
height: 0;
border-left: 5px solid transparent;
border-right: 5px solid transparent;
margin-left: 118px;
border-top: 5px solid white;
}
.banner-dots-2{
width: 300px;
height: 300px;
margin : -200px auto;
position: relative;
}
.banner-dots-2 img{
max-height: 300px;
max-width: 300px;
}
.banner-dots-2 button{
position: absolute;
left: 50%;
transform: translate(-50%, 0);
bottom: 20px;
width: 50px;
height: 50px;
vertical-align: center;
border-radius: 25px;
background-color: #77c977;
color: white;
border: none;
font-weight: 300;
font-size: 16px;
}
.manage-header{
color: #254266

}
.active-1{
  margin-top: 40px;
}
.active-1-left{
  margin: 100px auto;
  max-width: 850px;
  padding-left: 20%;
}
.active-1-left button{
  transition: 0.3s;
}
.active-1-left button:hover{
  border: 2px solid #77c977;
  color: #77c977;
  transition: 0.3s;
  background-color: white;
}
.view-review{
  transition: 0.3s;
}
.view-review:hover{
  border: 2px solid #77c977;
  color: #77c977;
  transition: 0.3s;
  background-color: white;
}
.active-1-left h1{
  position: relative;
  padding-bottom: 10px;
  font-size: 34px;
  text-align: left;
  width: 100%;
  font-family: 'Poppins', sans-serif;
font-size : 45px;
color: #254266;
font-weight: 400;
  margin-bottom: 20px;
  }
.active-1-left h1:after{
  content: "";
  background: #77c977;
  position: absolute;
    left: 0;
    bottom: 0;
    width : 10%;
    height: 2px;
}
.active-1-left p{
  text-align: left;
  font-size: 17px;
  color: #757575;
  line-height: 1.94;
}
.active-1-right{
  padding-left: 150px;
  margin: 20px auto;

}
.active-1-right img{
  z-index: 200;
  max-width: 100%;
  max-height: 100%;
  position: relative;
}
.active-1-float{
  position: absolute;
  z-index: 250;
  left: 0;
  bottom: -10%;
}
.active-1-float1{
  width: 300px;
  height: 140px;
  background-color: #FDFDFD;
  
}
.pulsating-circle {
  position: absolute;
  left: 0;
  top: 25%;
  transform: translateX(-50%) translateY(-50%);
  width: 80px;
  height: 80px;
}
  
 .pulsating-circle:before {
    content: '';
    position: relative;
    display: block;
    width: 150%;
    height: 150%;
    box-sizing: border-box;
    margin-left: -25%;
    margin-top: -25%;
    border-radius: 80px;
    background-color: #77c977;
    
    animation: pulse-ring 1.5s cubic-bezier(0.215, 0.61, 0.355, 1) infinite;
  }
  
  .pulsating-circle:after {
    font-family: FontAwesome;
    content: '\f00c';
    position: absolute;
    left: 0;
    top: 0;
    font-weight: 100;
    text-align: center;
    padding-top: 18px;
    font-size: 30px;
    color: white;
    display: block;
    width: 100%;
    height: 100%;
    background-color: #77c977;
    border-radius: 60px;
    box-shadow: 0 0 8px rgba(0,0,0,.3);
    animation: pulse-dot 1.5s cubic-bezier(0.455, 0.03, 0.515, 0.955) -.4s infinite;
  }


@keyframes pulse-ring {
  0% {
    transform: scale(.33);
  }
  80%, 100% {
    opacity: 0;
  }
}

@keyframes pulse-dot {
  0% {
    transform: scale(.8);
  }
  50% {
    transform: scale(1);
  }
  100% {
    transform: scale(.8);
  }
}
.active-1-float1 h4{
  padding-top: 24px;
  padding-left: 50px;
  font-size: 16px;
  font-weight: 400;
  color : #58595a;
}
.active-1-float1 a{
  color: #26a9e1;
  padding-left: 50px;
  font-size: 18px;
}
.active-1-float2{
  padding-top : 15px;
  padding-left: 20px;
  padding-right: 20px;
  width: 350px;
  height: 140px;
  right: 30%;
  background-color: #ffffff;
}
.active-1-float2 p{
  padding-bottom: 10px;
  font-size: 12px;
  color: #757575;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}
.active-1-float2 img{
  float: right;
  z-index: 300;
}
.active-1-float2 h4{
  padding-top: 20px;
  font-size: 14px;
  color: #757575;
}
.active-1-float2-payment{
  flex-direction: row;
  justify-content: space-between;
}
.active-1-float2 h3{
  text-align: center;
  width: 80px;
  line-height: 34px;
  margin-top: 10px;
  height: 34px;
  font-size: 16px;
  border-radius: 5px;
  background-color: #f5fafc;
}
.active-1-dots{
  right: 20%;
  margin-top: 30%;
  position: absolute;
  z-index: 50;
}
.active-1-dots img{
  max-width: 70%;
  max-height: 70%;
}
.active-2{
  margin-top: 250px;
}
.active-2-right{
  padding-left: 100px;
  max-width: 550px;
  margin-top: 200px;
}
.active-2-right h1{
  position: relative;
  padding-bottom: 10px;
  font-size: 40px;
  text-align: left;
  width: 100%;
  color: #254266;
  font-family: 'Poppins', sans-serif;
font-size : 45px;
font-weight: 400;
  margin-bottom: 20px;
  }
.active-2-right h1:after{
  content: "";
  background: #77c977;
  position: absolute;
    left: 0;
    bottom: 0;
    width : 10%;
    height: 2px;
}
.active-2-right p{
  text-align: left;
  font-size: 14px;
  color: #757575;
}
.active-2-left img{
  float: right;
  
  z-index: 300;
  position: relative;
}
.active-2-blue{
  width: 60%;
  height: 600px;
  position: absolute;
  left: -15px;
  margin-top: 10%;
  z-index: 100;
  background-color: #eef3fa;
}
.active-2-textbox1{
  width: 85px;
  height: 52px;
  border-radius: 5px;
  left: 24%;
  font-size: 15px;
  line-height: 52px;
  text-align: center;
  background-color: white;
  margin-bottom: 10px;
  margin-left: 10px;
  z-index: 400;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);

}
.active-2-textbox2{
  width: 303px;
  height: 100px;
  border-radius: 5px;
  left: 26%;
  font-size: 15px;
  padding-top: 15px;
  padding-left: 10px;
  padding-right: 10px;
  text-align: left;
  background-color: white;
  z-index: 400;
  margin-bottom: 10px;
  margin-left: 30px;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);

}
.active-2-textbox3{
  width: 300px;
  left: 26%;
  font-weight: 600;
  font-size: 12px;
  padding-left: 10px;
  padding-right: 10px;
  color : #1c2e40;
  z-index: 400;
  margin-left: 30px;
  margin-bottom: 20px;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);

}
.active-2-textbox{
  position: absolute;
  z-index: 700;
  right: 28%;
  margin-top: 20%;
}
.active-2-textbox-float{
  display: flex;
  flex-direction: row;
}
.active-2-user{
  width: 40px;
  height: 40px;
  background-color: #77c977;
  border-radius: 20px;
  line-height: 40px;
  text-align: center;
  color: white;
  z-index: 400;
  font-size: 16px;
  margin-right: 10px;
  left: 23%;
}
.active-2-textbox4{
  width: 358px;
  height: 120px;
  border-radius: 5px;
  left: 28%;
  font-size: 15px;
  padding-top: 15px;
  padding-left: 10px;
  padding-right: 10px;
  text-align: left;
  background-color: white;
  z-index: 400;
  line-height: 1.47;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);

}
.active-2-textbox5{
  width: 237px;
  height: 51px;
  font-weight: 600;
  font-size: 12px;
  padding-top: 15px;
  padding-left: 10px;
  padding-right: 10px;
  color : #1c2e40;
  z-index: 400;
  margin-left: 40px;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);


}
.active-2-textbox6{
  width: 250px;
  height: 51px;
  border-radius: 5px;
  font-size: 15px;
  padding-top: 15px;
  padding-left: 10px;
  padding-right: 10px;
  text-align: left;
  background-color: white;
  z-index: 400;
  margin-left: 60px;
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);

}
.active-2-textbox6 img{
  float: right;
}
.service-right{
  height: 800px;
  padding-top: 100px;
}
.service-right h1{
  font-size: 36px !important;
}
.service-1{
  margin-top: 5%;
  
}
.service-2{
  
  margin-top: 10%;
}

.service-3{
  margin-left: 10%;
  
  margin-top: 10%;
}

.service-4{
  margin-left: -5%;
  margin-top: 10%;
}

.service-wrap{
  position: absolute;
  width: 80%;
  display: flex;
  flex-direction: row;
  z-index: 250;
  left: 30%;
  flex-wrap: wrap;
  padding-top: 200px;
  justify-content: space-around;
}
.service-left img{
  max-width: 100%;
  max-height: 100%;
}
.service-wrap>div{
  flex: 0 40%;
  width: 100%;
}
.service-btn{
  width: 30%;
  height: 7%;
  background-color: white;
  position: absolute;
  display: flex;
  left: 20%;
  margin-top: -5%;
  font-family: "Poppins";
  font-size: 20px;
  font-weight: 500;
  flex-direction: row;
  border-radius: 5px;
  padding-left: 10px;
  transition: 0.1s;
  box-shadow: 0px 5px 30px 0 rgba(0, 0, 0, 0.07);
}
.service-2>.service-btn{
  left: 65%;
  width: 35%;

  margin-top: -5%;
}
.service-btn h3{
  text-align: center;
  font-size: 1vw;
  border-radius: 5px;
  margin: 0 auto;
  padding-top: 10%;
}
.service-btn button{
  border: none;
  width: 40px;
  height: 40px;
  margin: auto;
  color: #636363;
}
.service-btn:hover{
  border-bottom: 5px solid #77c977;
  transition: 0.1s;
}
.service-btn:hover >button{
  background-color: #EEFBF1;
  color: #77c977;

}

.service-3>.service-btn{
  width: 35%;
  height: 7%;
}
.service-4>.service-btn{
  width: 22% !important;
  height: 6% !important;
  left: 60%;
  margin-top: -3%;
}
.service-4-btn h3{
  font-size: 0.8vw;
  padding-top: 13%;
}
.instructions-left{
  height: 600px;
  z-index: 200;
  padding-top: 100px;
}
.instructions-left-wrap{
  width: 60%;
  margin: 80px auto;
}
.instructions-left-wrap p{
  margin-top: 50px;
}
.instructions-left button{
  background-color: #77c977;
  text-align: center;
  color: #ffffff;
  font-weight: bold;
  font-size: 12px;
  height: 60px;
  width: 220px;
  margin-top: 50px;
  border: none;
  font-size: 16px;
}
.instructions-left i{
  padding-left: 20px;
}
.instructions-green{
  width: 80%;
  height: 800px;
  position: absolute;
  left: -15px;
  z-index: 100;
  background-color: #EEFBF1;
}
.instructions-wrap{
  position: relative;
  z-index: 500;
  width: 100%;
  height: 100%;
}
.instructions-item{
  width: 280px;
  position: absolute;
  height: 230px;
  background-color: white;
  border-radius: 5px;
  text-align: center;
  padding-top: 30px;
  padding-left: 20px;
  padding-right: 20px;
  box-shadow: 3.9px 4.6px 20px 0 rgba(0, 0, 0, 0.05);
}
.instructions-item p{
  padding-top: 20px;
  font-family: "Poppins";
  font-weight: 500;
  line-height: 1.72;
  font-size: 18px;
  color: black;
  text-align: center;
}
.ins-item1{
  left: -80%;

  border-bottom: 5px solid #77c977;
}
.ins-item1 p{
  color: #77c977;
}
.ins-item2{
  margin-top: -30%;
}
.ins-item3{
  margin-top : 40%;
}
.contract-rating{
  display: flex;
  flex-direction: row;
  line-height: 70px;
  color: #77c977;
  font-weight: 800;
  font-size: 30px;
}
.contract-rating div{
  width: 70px;
  height: 70px;
  border-radius: 30px;
  background-color: #FFE9BF;
  padding-left: 18px;
  margin-right: 20px;
}
.contract-left{
  padding-left: 10%;
}
.con-1{
  right: -20%;
}
.con-2{
  right: -20%;
  margin-top: 50%;
}
.con-3{
  left: -20%;
  margin-top: 30%;
}
.contract-left>img{
  max-width: 120%;
  max-height: 120%;
}
.contractors{
  margin-top: 10%;
}
.contractor-wrap{
  z-index: 500;
  margin: 0 auto;
  width: 60%;
  margin-top: -60%;
  position: absolute;
}
.contractor{
  max-width: 200px;
  max-height: 200px;
  position: absolute;
  background-color: white;
  border-radius: 5px;
  box-shadow: 0px 17px 20px 0 rgba(0, 0, 0, 0.05);
  z-index: 500;
  text-align: center;
  padding-top: 15px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
}
.contractor div{
  font-size: 30px;
  font-weight: 900;
  
}
.contractor img{
  max-width: 100%;
  max-height: 100%;
}
.contractor h4{
  font-size: 22px;
}
.contractor h5{
  font-size: 16px;
  color: #8c9aa3;
  margin-bottom: 0px;
}

.client{
  position: relative;
  margin-top: 0px !important
}
.client h1{
  padding-top: 100px;
}
.client-blue{
  position: absolute;
  right: 0;
  width: 80%;
  height: 800px;
  background-color: #eef3fa;
}
.client-wrapper{
  z-index: 600;
  width: 80%;
  padding-top: 40px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin : 0 auto;
}
.client-item{
  width: 30%;
  max-height: 500px;
  min-height: 250px;
  position: relative;
  background-color: white;
  border-radius: 10px;
  padding-bottom: 20px;
  box-shadow: 3.9px 4.6px 20px 0 rgba(0, 0, 0, 0.05);
}
.client-content{
  display: flex;
  flex-direction: row;
  padding-left: 10px;
  padding-right: 10px;
  padding-top: 20px;
  padding-bottom: 120px;
}
.client-content span{
  padding-left: 20px;
  text-align: left;
  width: 80%;
  font-size: 16px;
  color: #757575;

}
.client-content img{
  max-width: 30px;
  max-height: 22px;
}
.client-info{
  position: absolute;
  bottom: 5%;
  padding-left: 5%;
  margin-top: 5%;
  display: flex;
  flex-direction: row;
}
.client-info h3{
  font-size: 18px;
}
.client-info div{
  padding-left: 20px;
}
.client-info span{
  font-size: 14px;
  color: #757575;
}
.client-info div>img{
  width: 148px;
  height: 24px;
}
.view-review{
  box-shadow: 49.5px 49.5px 66.5px 3.5px rgba(0, 0, 0, 0.15);
    background-color: #77c977;
  text-align: center;
  color: #ffffff;
  font-size: 16px;
  height: 60px;
  width: 220px;
  border: none;
  position: absolute;
  z-index: 600;
  left: 15%;
  bottom: -20%;
}
.view-review i{
  padding-left: 20px;
}
.question{
  margin-top: 400px;
}
.question-left{
  padding-left: 10% !important;
}
.card-header {
  position: relative;
  max-height: 100px;
  padding-left: 20px;
  font-family: "Poppins";
  font-size: 18px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.72;
  background-color: white;
  border: none;
}
  
.card-header::after {
  text-align: center;
	content: "\f063";
  color: #333;
  margin-left: 30px;
	top: -2px;
  right: 0px;
  width: 40px;
  padding-left: 12px;
  line-height: 40px;
  height: 40px;
	position: absolute;
  font-family: "FontAwesome";
    padding-right: 20px;
    border-radius: 3px;
    background-color: #F7F7F7;
}


.card-header[aria-expanded="true"]{
  color: #77c977;
}
.card-header[aria-expanded="true"]::after {
  content: "\f062";
  background-color: #F7F7F7;
  color: #77c977;
}
.card-body{
  padding-left: 40px;
  padding-right: 140px;
  padding-bottom: 20px;
  padding-top: 30px;
  margin-top: -10px;
  font-family: "Poppins";
  font-size: 17px;
  font-weight: 300;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.76;
  letter-spacing: 0.51px;
  text-align: left;
  color: #868686;
  background-color: white;
  border-bottom: 5px solid #77c977 ;
  border-radius: 0 0 5px 5px;
  border-top: none;
  box-shadow: 3.9px 4.6px 21px 0 rgba(0, 0, 0, 0.07);

}
.card{
  margin-bottom: 20px;
  border: none;
}

.question-wrap{
  width: 70%;
  margin: 100px auto;
  padding-right: 60px;
  
}
.join-with-us-left{
  font-family: "Poppins";
  font-size: 40px;
  font-weight: normal;
  font-stretch: normal;
  margin: 0 auto !important;
  font-style: normal;
  line-height: 1.18;
  letter-spacing: 1.2px;
  padding-left: 8% !important;
}
.join-with-us-left h1{
  font-size: 40px;
}
.join-with-us-left p{
  width: 70%;
}
.join-with-us-right{
  margin: 0 auto;
}
.join-with-us-right button{
  width: 172px;
  height: 56px;
  border: 2px solid #77c977;
  background-color: white;
  color: #77c977;
  font-family: "Poppins";
  font-size: 18px;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.33;
  transition: 0.3s;
  margin-right: 20px;
}
.join-with-us-right button:hover{
  color: white;
  background-color: #77c977;
  transition: 0.3s;
}
.join-with-us-right i{
  padding-left: 10px;
}
.footer-1{
  margin: 100px auto;
  margin-bottom: 0px;
  padding-left: 0px;
  background-color: #151a2d;
  border-bottom: 1px solid #2d3142;
}
.footer-1-left{
  padding-left: 10% !important;
  margin-left: 0px;
}
.footer-1-left h1{
  color: white;
  font-family: "Poppins";
  font-size: 40px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.38;
  letter-spacing: 1.2px;
}
.footer-1-right{
  width: 70%;
  margin: 100px auto;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
.footer-1-right input{
  background-color: #151a2d;
  border: 1px solid #2d3142;
  color: #2d3142;
  height: 56px;
  opacity: 0.6;
  font-family: "Poppins";
  font-size: 17px;
  font-weight: 300;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.41;
  letter-spacing: 0.51px;
  text-align: center;
  color: rgba(255, 255, 255, 0.6);
  text-align: left;
  padding-left: 20px;
  max-width: 250px;
}
.footer-1-right i{
  padding-left: 10px;
}
.footer-1-right button{
  width: 172px;
  height: 56px;
  color: white;
  background-color: #77c977;
  transition: 0.3s;
  font-family: "Poppins";
  font-size: 18px;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.33;
  transition: 0.3s;
  margin-right: 20px;
  border: none;
}
.footer-1-right button:hover{
  color: #77c977;
  background-color: white;
  transition: 0.3s;
  border: 2px solid #77c977;
}
.footer-2{
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  background-color: #151a2d;
  padding-top: 50px;
}
.footer-2-item{
  color : white;
}
.footer-2-item li{
  list-style: none;
  margin-bottom: 10px;
}
.footer-2-item ul{
  padding-left: 0px;
  margin-top: 20px;
}
.footer-2-item a{
  color: rgba(220, 220, 220, 0.3);
  transition: 0.3s;

}
.footer-2-item a:hover{
  text-decoration: none;
  color: white;
  transition: 0.3s;
}
.footer-2-item i{
  padding-left: 10px;
}
.footer-3{
  width: 100%;
  height: 250px;
  display: flex;
  background-color: #151a2d;
  flex-direction: row;
  padding-top: 40px;
  position: relative;
}
.footer-3-wrap{
  width: 84%;
  border-top: 1px solid rgba(220, 220, 220, 0.3);
  margin: 0 auto;
  padding-top: 40px;

  display: flex;
  background-color: #151a2d;
  flex-direction: row;
  justify-content: space-between;
}
.footer-3-left h5{
  font-family: "Poppins";
  font-size: 18px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.67;
  letter-spacing: 0.54px;
  text-align: left;
  color: rgba(220, 220, 220, 0.3);
}
.footer-icon{
  width: 50px;
  height: 48px;
  border-radius: 5px;
  margin-right: 20px;
  font-size: 27px;
  text-align: center;
  line-height: 48px;
  color: white;
  background-color: #2E2F42;
  transition: 0.3s;
}
.fb-icon:hover{
  background-color: #3b5998;
  transition: 0.3s;
}
.twitter-icon:hover{
  background-color: #1da1f2;
  transition: 0.3s;
}
.ins-icon:hover{
  background-color: #c13584;
  transition: 0.3s;
}
.in-icon:hover{
  background-color: #2867b2;
  transition: 0.3s;
}
.footer-3-right{
  display: flex;
  flex-direction: row;
}
.footer-3-left span{
  color: #77c977;
  font-weight: bold;
  text-transform: uppercase;
}
.scroll-btn{
  position: fixed;
  right: 50px;
  bottom: 100px !important;
  width: 50px;
  height: 50px;
  background-color: #77c977;
  color: white;
  z-index: 1000;
  border: none;
}
.bounce-up{
  opacity: 0;
  -moz-transition: all 700ms ease-out;
  -webkit-transition: all 700ms ease-out;
  -o-transition: all 700ms ease-out;
  transition: all 700ms ease-out;
  -moz-transform: translate3d(0px, 250px, 0px);
  -webkit-transform: translate3d(0px, 250px, 0px);
  -o-transform: translate(0px, 250px);
  -ms-transform: translate(0px, 250px);
  transform: translate3d(0px, 250, 0px);
  -webkit-backface-visibility: hidden;
  -moz-backface-visibility: hidden;
  backface-visibility: hidden;
}
.slide-left {
  opacity: 0;
  -moz-transition: all 500ms linear;
  -webkit-transition: all 500ms linear;
  -o-transition: all 500ms linear;
  transition: all 500ms linear;
  -moz-transform: translate3d(-100px, 0px, 0px);
  -webkit-transform: translate3d(-100px, 0px, 0px);
  -o-transform: translate(-100px, 0px);
  -ms-transform: translate(-100px, 0px);
  transform: translate3d(-100px, 0px, 0px);
}
.slide-right{
  opacity: 0;
  -moz-transition: all 500ms linear;
  -webkit-transition: all 500ms linear;
  -o-transition: all 500ms linear;
  transition: all 500ms linear;
  -moz-transform: translate3d(200px, 0px, 0px);
  -webkit-transform: translate3d(200px, 0px, 0px);
  -o-transform: translate(200px, 0px);
  -ms-transform: translate(200px, 0px);
  transform: translate3d(200px, 0px, 0px);
}
.in-view{
  opacity: 1;
  -moz-transform: translate3d(0px, 0px, 0px);
  -webkit-transform: translate3d(0px, 0px, 0px);
  -o-transform: translate(0px, 0px);
  -ms-transform: translate(0px, 0px);
  transform: translate3d(0px, 0px, 0px);
}
@media (max-width: 1200px) {
  .active-1-right{
    padding-left: 5%;
  }
  
  .client-wrapper{
    justify-content: right;
    flex-wrap: wrap;
  }
  .client-item{
    float: right;
    margin-top: 10px;
    width: 60%;
  }
  .view-review{
    bottom: 30%;
  }
  .ins-item1{
    top: -20%;
    left: 0;
  }
  .ins-item2{
    top: 30%;
    margin-top: 0px;
  }
  .ins-item3{
    margin-top: 0px;
    top: 80%;
  }
  .num-3{
    visibility: hidden;
  }
  .con-1{
    left: -20%;
    margin-top: -50%;
  }
  .con-2{
    right: -50%;
    margin-top: 0;
  }
}

</style>
