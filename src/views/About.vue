<template>
  <div class="about page">
    <div class="aboutComponent">


      <img src="../assets/pp.jpg" alt="">
    <Test title="Sabir Barahi" >

      <template v-slot:info>
        <p>I'm a student currently studying Computer Programming at 東京デザインテクノロジーセンター専門学校 in Japan. I have been studying and living in Japan for three years. I love to code,
          do web development projects and constantly learn new things.
        </p>
      </template>

      <template v-slot:info2>
        <p>
          I was born in Nepal, the country of Mount Everest. My family has a Technical background and I have always been around innovative people. I'm naturally curious and love trying out new things. I love music, playing guitar and singing.
          I grew up building the <a href="https://en.wikipedia.org/wiki/Rato_Machindranath_Jatra" style="color:white">Chariot of Machindranath.</a>  
        </p>
      </template>



    </Test>
</div>
  </div>
</template>

<script>
import Test from "../components/Test";



export default {
  
  name: 'About',
  
  components:{
    Test
    }
    }
</script>





<style>
*{
margin: 0;
padding: 0;
}
.about{
  position: absolute;
  background: #293241;
  color: #faf9f9;
  height: 100%;
  width: 100%;
}

.about a{
  color:white;
}

.aboutComponent{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  animation: bounce 1s ease;
}

.aboutComponent h1{

  padding: 20px;
  font-size: 2em;
  
}

.aboutComponent p{

  font-size: 1em;
  
}
.aboutComponent img{
  border: 5px whitesmoke solid;
  border-radius:50%;
  width: 15%;
}
@media(max-width:900px){
  .aboutComponent img{
    position: absolute;
    width: 50%;
  }
.aboutComponent p{

  font-size: 2em;
  
}
.aboutComponent h1{
  visibility: hidden;
}
}

@keyframes bounce {
  0%{
    transform: translateY(-100px);
  }
  50%{
    transform: translateY(20px);
  }
  100%{
    transform: translateY(0);
    
  }
}

</style>


