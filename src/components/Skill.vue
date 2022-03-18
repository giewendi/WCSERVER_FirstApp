<template>
  <div id="Skills">
    <h2>{{ title }}</h2>
    <div id="skill">
        <ul>
            <li>{{skill1}}<input type="range" id="aa" min="0" max="100" step="1"></li>
            <li>{{skill2}}<input type="range" id="ab" min="0" max="100" step="1"></li>
            <li>{{skill3}}<input type="range" id="ac" min="0" max="100" step="1"></li>
            <li>{{skill4}}<input type="range" id="ad"  min="0" max="100" step="1"></li>
            <li>{{skill5}}<input type="range" id="ae" min="0" max="100" step="1"></li>
            <li>{{skill6}}<input type="range" id="af" min="0" max="100" step="1"></li>
        </ul>
    </div>

    <div id="comp">
        <ul>
            <li><img src="./assets/powerpoint.png" alt="Microsoft Office Icon"><p>{{tool1}}</p></li>
            <li><img src="./assets/photoshop.png" alt="Photoshop Icon"> <p>{{tool2}}</p></li>
            <li><img src="./assets/montage.png" alt="Video Edit Icon"> <p>{{tool3}}</p></li>
            <li><img src="./assets/html.png" alt="HTML Icon"> <p>{{tool4}}</p></li>
            <li><img src="./assets/python.png" alt="Python Icon"> <p>{{tool5}}<br>{{prog1}} | {{prog2}}</p></li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skill',
  data () {
    return {
      title: 'Skill',
      skill1: 'Effective Listening and Comprehension',
      skill2: 'Respectful and Professionalism',
      skill3: 'Effective Communication',
      skill4: 'Team Player / People Skill',
      skill5: 'Computer and Technology Literate',
      skill6: 'Multitasking / Time Management',
      tool1: 'Microsoft Office Tools',
      tool2: 'Photoshop',
      tool3: 'Basic Video Editing',
      tool4: 'HTML, CSS and JavaScript',
      tool5: 'Programming',
      prog1: 'Python',
      prog2: 'Java',
    }
  }
}
</script>

<style>
#skill input[type="range"]{
    -webkit-appearance: none;
    margin-right: 15px;
    width: 300px;
    height: 10px;
    background: rgba(255, 255, 255, .9);
    border-radius: 5px;
    background-image: linear-gradient(#3D3122, #3D3122);
    background-repeat: no-repeat;
}

#skill input[type="range"]#aa{background-size: 80% 100%;}
#skill input[type="range"]#ac{background-size: 80% 100%;}
#skill input[type="range"]#ad{background-size: 95% 100%;}
#skill input[type="range"]#ae{background-size: 100% 100%;}
#skill input[type="range"]#af{background-size: 75% 100%;}

#skill input[type="range"]::-webkit-slider-thumb {
    display: none;
}

#skill li{
    text-align: center;
    width: 25em;
    margin: 1em;
    padding: 1em 2em;
    background-color: rgba(207, 156, 61, 0.40);
    filter: drop-shadow(0 0 1px rgb(56, 54, 51));
    color: #fff;
    font-size: large;
}

#skill ul{
    overflow: auto;
    list-style-type: none;
    margin: 1em 0 0 ;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    flex: 50%;
}

#comp li{
    text-align: center;
    width: 25em;
    margin: 1em;
    padding: 1em 2em;
    background-color: rgb(255, 255, 255);
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
    font-size: large;
}

#comp ul{
    overflow: auto;
    list-style-type: none;
    margin: 1em 0 0 ;
    display: flex;
    justify-content: center;
}

#comp img{
    width: 100px;
}

#work div{
    display: flex;
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
}

#work img{
    margin: 0 10%;
    width: 30%;
    border: 20px solid white;
}

#work section img{
    margin: 3em 0 0;
    width: 80%;
}

#work section{
    text-align: center;
}

#work p{
    margin: 10% 0 0;
    background: white;
    font-size: larger;
    padding: 1em;
}
</style>