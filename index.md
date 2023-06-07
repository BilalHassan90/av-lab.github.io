---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<h1 class='av-title'>Autonomous Vehicle Lab
</h1>
<img class="small-banner"/> 
<div class="wrapper2">
<!-- <div class="video-background">
  <video autoplay loop muted playsinline preload="auto">
    <source src="/assets/bg-anim.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div> -->
<div class="left-column">
  <p class="sum">
  <img src="/assets/img/logo.png" width="90px" class="logo"/>
    Welcome to the Autonomous Vehicle Lab (AV-Lab) at <a href="https://ku.ac.ae" target="_blank" rel="noopener noreferrer">Khalifa University</a>. Our research focuses on the safe operation of AVs, their integration into intelligent urban environments, and the AI alignment for embodied AI systems, specifically in the context of AVs.
  </p>
  <div class="questions">
  <p> We address the following pivotal questions: </p>
    <ul>
      <li>How can safety be ensured within the core components of the AV decision-making pipeline?</li>
      <li>How can AV components effectively exchange and interpret uncertainties from the environment while harnessing Vehicle-to-Everything (V2X) technology for multi-agent solutions?</li>
      <li>How can decision-making frameworks effectively combine the benefits of machine learning and the rigor of theoretical computer science to create verifiably safe solutions?</li>
      <li>Can we align AV goals with human values and expectations?
      </li>
    </ul>
  </div>


  
</div>
  <div class="right-column">
      <img class='banner'/>
  </div>
</div>

<style>
.av-title{
     margin-bottom:-20px;
    margin-top: -15px;
    font-size: 40.5px;   
}
.logo{
  float: left;
  padding-right:5px;
  margin-top: -11px;
  margin-left: -11px;
}
.logo:hover{
  filter: hue-rotate(180deg);
}
.wrapper2 {
  display: flex;
  justify-content: space-between;
  align-items: stretch;
  position: relative;
  overflow: hidden;
}

.video-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
}

.video-background video {
  min-width: 100%;
  min-height: 100%;
  object-fit: cover;
}

.left-column,
.right-column {
  display: flex;
  flex-direction: column;
  position: relative;
  height: 100%; /* Add this line */
  hyphens: auto;
  text-align: justify;
}

.left-column {
  flex: 60%;
}

.right-column {
  flex: 40%;
  /* margin-top:-65px; */
}

.left-column ul {
  list-style-type: "‣ ";
  margin-top: -10px;
  margin-bottom: -10px;
}
.left-column li {
  padding-bottom: 10px;
}
.sum{
    margin-top: 15px;
    margin-bottom: 0px;
    color:#838996;
    background-color:#f5f5f5;
    padding: 15px;
    padding-left: 20px;
    padding-right: 25px;
}

.sum:hover{
    background-color:#f8f8ff;
}
.questions{
  background-color: #f9fbff ;
  color:#566968 ;
  padding: 12px;
  
  padding-right: 25px;
}
.questions:hover{
  opacity: 80%;
    background-color: #566968 ;
    color:#f9fbff;
}


.banner{
    content: url("/assets/banner-anim.gif");
    width:100%; 
    margin:0px;
    margin-top:13px;
}

.banner:hover{
    opacity:0.8;
}
.video{
    margin:0;
    margin-bottom: 0px;
    margin-top: 10px;
    width:100%; 
}
.ads:hover{
    opacity:0.8;
}


a{
    color: black;
}
.small-banner{
  display: none;
  margin: 0;
  padding: 0;
}

@media (max-width: 600px) {
  .wrapper2 {
    display: flex;
    justify-content: space-between;
    position: relative;
    z-index: 1;
  }

  .right-column {
    width: 100%;
  }
  .right-column {
    display: none;
  }

  .small-banner{
      content: url("/assets/img/banner-small.png");
      margin-top: 15px;
      display: inline-block;
  }

}



</style>
