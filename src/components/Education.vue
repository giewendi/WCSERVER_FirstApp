<template>
  <div id="Education">
      <h2>{{title}}</h2>
      <div id="educ">
        <input type="radio" id="tab1" name="t" checked>
            <label for="tab1">{{collegeDate}}</label>
            <section class="tab">
                <h3>{{collegeDate}}</h3>
                <div>
                    <img src="./assets/hau.png" alt="HAU Logo" width="200px">
                    <p><b>{{collegeSchool}}</b><br>
                        1st Year and 2nd Year First Semester<br>
                        BS Information Technology - Web Development</p>
                </div>
            </section>
            <input type="radio" id="tab2" name="t">
            <label for="tab2">{{shsDate}}</label>
            <section class="tab">
                <h3>{{shsDate}}</h3>
                <div>
                    <img src="./assets/hau.png" alt="HAU Logo" width="200px">
                    <p><b>{{shsSchool}}</b><br>
                        Senior High School<br>
                        Science, Technology, Engineering and Mathematics</p>
                </div>
            </section>
            <input type="radio" id="tab3" name="t">
            <label for="tab3">{{jhsDate}}</label>
            <section class="tab">
                <h3>{{jhsDate}}</h3>
                <div>
                    <img src="./assets/dalcuis.jpg" alt="HAU Logo" width="200px">
                    <p><b>{{jhsSchool}}</b><br>
                        Elementary and Junior High School<br>
                        Grade 2 - Grade 10</p>
                </div>
            </section>
            <input type="radio" id="tab4" name="t">
            <label for="tab4">{{elemDate}}</label>
            <section class="tab">
                <h3>{{elemDate}}</h3>
                <div>
                    <img src="./assets/sto.jpg" alt="HAU Logo" width="200px">
                    <p><b>{{elemSchool}}</b><br>
                        Grade School - Grade 1 <br>
                        Preparatory School</p>
                </div>
            </section>
        </div>
  </div>
</template>

<script>
export default {
  name: 'Education',
  data () {
    return {
      title: 'Educational Background',
      collegeDate: '2021-2020',
      shsDate: '2020-2018',
      jhsDate: '2018-2009',
      elemDate: '2009-2007',
      collegeSchool: 'Holy Angel University',
      shsSchool: 'Holy Angel University',
      jhsSchool: 'Don Antonio Lee Chi Uan Integrated School',
      elemSchool: 'Santo Rosario Elementary School'
    }
  }
}
</script>

<style>
#educ{
    display: flex;
    flex-wrap: wrap;
    max-width: 80%;
    margin: 50px auto;
    margin-top: 0;
    padding: 25px;
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
}

#educ input[type="radio"]{
    display: none;
}

#educ label{
    padding: 25px 5%;
    background: rgba(207, 156, 61, 0.40);
    font-weight: bold;
    color: white;
}

#educ .tab{
    width: 100%;
    padding: 2% 5% 5%;
    background: #fff;
    order: 1;
    display: none;
}

#educ .tab h2 {
    font-size: 2.5em;
    margin-left: 10%;
}

#educ input[type='radio']:checked + label + .tab{
    display: block;
}

#educ input[type='radio']:checked + label{
    background: #fff;
    color: rgb(61, 49, 34);
}

#title, #skill h1, #work h1, #cert h1{
    background-color: rgb(255, 255, 255);
    padding: 7px;
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
    margin-top: 1.5em;
    text-align: center;
}

#educ div{
    display: flex;
    align-items: center;
    font-size: 1.5em;
}

#educ img{
    margin: 0 10%;
}
</style>