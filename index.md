---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<h1 class='av-title'>Autonomous Vehicle Lab </h1>
<div class="wrapper2">
<!-- <div class="video-background">
  <video autoplay loop muted playsinline preload="auto">
    <source src="/assets/bg-anim.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div> -->
<div class="left-column">
  <p class="sum">
    Welcome to the Autonomous Vehicle Lab (AV-Lab) at <a href="https://ku.ac.ae">Khalifa University</a>. Our  research centers around Autonomous Vehicle (AV) technologies, safety assurance, integration into intelligent urban environments, and AI alignment for embodied AI systems.
  </p>
  <img class="small-banner"/> 
  <p>We address the following pivotal questions:</p>
  <ul>
    <li>How can safety be ensured within the core components of the AV decision-making pipeline?</li>
    <li>How can components effectively exchange and interpret uncertainties while harnessing V2X technology for multi-agent solutions?</li>
    <li>How can decision-making frameworks be developed that amalgamate the advantages of machine learning and the rigor of theoretical computer science to produce demonstrably safe solutions?</li>
    <li>How can we align AV goals with human values and expectations?
    </li>
  </ul>


  
</div>
  <div class="right-column">
      <img class='banner'/>
  </div>
</div>

<style>
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
}

.left-column {
  flex: 60%;
}

.right-column {
  flex: 40%;
}

.left-column ul {
  margin-left: 20px;
  list-style-type: disc;
}

.av-title{
    margin-bottom:0px;
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
.sum{
    margin-top: 15px;
    color:#838996;
    background-color:#f5f5f5;
    padding:16px;
  
}
.sum:hover{
    background-color:#DCDCDC;
    background-color:#f8f8ff;
}
a{
    color: black;
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
      margin-top:0;
  }

}



</style>
