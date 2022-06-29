<script>
let index = 0;
$: place = index;

let word = {"data":[{"id":1,"attributes":{"definition":"to please","createdAt":"2022-05-16T01:01:40.251Z","updatedAt":"2022-05-16T02:10:12.283Z","MaleorPresent":"ਯੁਜਬੋ","FemaleorPast":"ਆਜ਼ਬਾ","Type":"Past / Present","DateAdded":null,"Lang":null}},{"id":2,"attributes":{"definition":"be amazed","createdAt":"2022-05-16T01:11:51.629Z","updatedAt":"2022-05-16T02:10:01.285Z","MaleorPresent":"ਤਾਜ਼ਾਬਾ","FemaleorPast":"ਤਾਜ਼ਾਬੂ","Type":"Past / Present","DateAdded":null,"Lang":null}},{"id":3,"attributes":{"definition":"amazing/spectacular","createdAt":"2022-05-16T01:15:40.897Z","updatedAt":"2022-05-16T02:10:06.824Z","MaleorPresent":"ਮੁਦਿਲ","FemaleorPast":"ਮੁਦਿਲੋਨ","Type":"Singular / Plural","DateAdded":null,"Lang":null}},{"id":4,"attributes":{"definition":"reverence / jaleel - majesty","createdAt":"2022-05-22T23:59:27.468Z","updatedAt":"2022-05-22T23:59:27.468Z","MaleorPresent":"ਅਜਿਾਲਾ","FemaleorPast":"ਜਲੀਲ","Type":"Male / Female","DateAdded":null,"Lang":null}},{"id":5,"attributes":{"definition":"sacred","createdAt":"2022-05-23T00:04:02.554Z","updatedAt":"2022-05-23T00:04:02.554Z","MaleorPresent":"ਮੁਕਾਦਿਸ","FemaleorPast":"ਮੁਕਾਦਿਸੋਲ","Type":"Male / Female","DateAdded":null,"Lang":null}},{"id":6,"attributes":{"definition":"beard","createdAt":"2022-06-02T17:23:16.190Z","updatedAt":"2022-06-02T17:23:16.190Z","MaleorPresent":"ਰੀਛ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Persian"}},{"id":7,"attributes":{"definition":"sand","createdAt":"2022-06-02T17:27:28.610Z","updatedAt":"2022-06-02T17:27:41.464Z","MaleorPresent":"ਰਿਗ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Persian"}},{"id":8,"attributes":{"definition":"food / nourishment","createdAt":"2022-06-02T17:35:46.550Z","updatedAt":"2022-06-02T18:49:46.106Z","MaleorPresent":"ਤਾਮ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":9,"attributes":{"definition":"diet / nutrition","createdAt":"2022-06-02T17:36:57.808Z","updatedAt":"2022-06-02T18:50:01.395Z","MaleorPresent":"ਰਿਦਾਓਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":10,"attributes":{"definition":"fire","createdAt":"2022-06-02T18:20:55.648Z","updatedAt":"2022-06-02T18:20:55.648Z","MaleorPresent":"ਨਾਰ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":11,"attributes":{"definition":"separate, detach, disconnect, break, dismiss","createdAt":"2022-06-02T18:22:11.950Z","updatedAt":"2022-06-02T18:22:11.950Z","MaleorPresent":"ਫਸਲੁਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":12,"attributes":{"definition":"enthusiasm, intense interest, heartiness","createdAt":"2022-06-02T18:23:23.819Z","updatedAt":"2022-06-02T18:23:23.819Z","MaleorPresent":"ਹੁਮਾਸ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":13,"attributes":{"definition":"fuel","createdAt":"2022-06-02T18:25:43.270Z","updatedAt":"2022-06-02T18:25:43.270Z","MaleorPresent":"ਵਾਕੋਡੂਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":14,"attributes":{"definition":"no","createdAt":"2022-06-02T18:29:39.341Z","updatedAt":"2022-06-02T18:29:39.341Z","MaleorPresent":"ਲਾ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":15,"attributes":{"definition":"good, welfare-giving, benevolent, charitable,","createdAt":"2022-06-02T18:33:53.992Z","updatedAt":"2022-06-02T18:33:53.992Z","MaleorPresent":"ਕਾਈਰੁਨ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":16,"attributes":{"definition":"clean","createdAt":"2022-06-02T18:38:00.313Z","updatedAt":"2022-06-02T18:38:00.313Z","MaleorPresent":"ਨਾਜ਼ੀਫ","FemaleorPast":"ਨੁਜ਼ਾਫਾਤ","Type":"Singular / Plural","DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":17,"attributes":{"definition":"put, set, position, lay, design","createdAt":"2022-06-02T18:40:41.970Z","updatedAt":"2022-06-02T18:40:41.970Z","MaleorPresent":"ਵਾਡਾ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":18,"attributes":{"definition":"work, action, business, job, labor","createdAt":"2022-06-02T18:41:45.526Z","updatedAt":"2022-06-02T18:41:45.526Z","MaleorPresent":"ਆਮੁਲਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":19,"attributes":{"definition":"request, demand, order, seek, require","createdAt":"2022-06-02T18:42:50.532Z","updatedAt":"2022-06-02T18:42:50.532Z","MaleorPresent":"ਤਾਲਿਬ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":20,"attributes":{"definition":"task, mission, job, function, assignment","createdAt":"2022-06-02T18:43:43.227Z","updatedAt":"2022-06-02T18:43:43.227Z","MaleorPresent":"ਮੋਹਿਮ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}},{"id":21,"attributes":{"definition":"function, job, position, office, service","createdAt":"2022-06-02T18:44:55.981Z","updatedAt":"2022-06-02T18:45:43.400Z","MaleorPresent":"ਵਾਬੀਫਾਤਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic"}}],"meta":{"pagination":{"page":1,"pageSize":25,"pageCount":1,"total":21}}}


let nextWord0 = word.data[index+1].attributes.MaleorPresent;
let nextWord1 = word.data[index+2].attributes.MaleorPresent;
let nextWord2 = word.data[index+3].attributes.MaleorPresent;
let nextWord3 = word.data[index+4].attributes.MaleorPresent;
let prevWord2 = '';
let prevWord1 = '';
let prevWord0 = '';

if (index > 0) {
  prevWord2 = word.data[index-1].attributes.MaleorPresent;
}
if (index > 1) {
  prevWord1 = word.data[index-2].attributes.MaleorPresent;
}
if (index > 2) {
  prevWord0 = word.data[index-3].attributes.MaleorPresent;
}

function indexIs(i){
  if (i == -1) {
    index = place-1;
    nextWord0 = word.data[index+1].attributes.MaleorPresent;
    nextWord1 = word.data[index+2].attributes.MaleorPresent;
    nextWord2 = word.data[index+3].attributes.MaleorPresent;
    nextWord3 = word.data[index+4].attributes.MaleorPresent;
    if (index > 0) {
      prevWord2 = word.data[index-1].attributes.MaleorPresent;
    }
    if (index > 1) {
      prevWord1 = word.data[index-2].attributes.MaleorPresent;
    }
    if (index > 2) {
      prevWord0 = word.data[index-3].attributes.MaleorPresent;
    }
  } else {
    index = place+i;
    nextWord0 = word.data[index+1].attributes.MaleorPresent;
    nextWord1 = word.data[index+2].attributes.MaleorPresent;
    nextWord2 = word.data[index+3].attributes.MaleorPresent;
    nextWord3 = word.data[index+4].attributes.MaleorPresent;
    if (index > 0) {
      prevWord2 = word.data[index-1].attributes.MaleorPresent;
    }
    if (index > 1) {
      prevWord1 = word.data[index-2].attributes.MaleorPresent;
    }
    if (index > 2) {
      prevWord0 = word.data[index-3].attributes.MaleorPresent;
    }
  }


  // Animate fade-in
  document.getElementById("desc").animate([
    { transform: 'translateY(-2px)' },
    { transform: 'translateY(0px)' }
  ], {
    duration: 2100,
  });
  document.getElementById("heading").animate([
    // keyframes
    { transform: 'translateY(-2px)' },
    { transform: 'translateY(0px)' }
  ], {
    // timing options
    duration: 2100,
  });


}
</script>

<html data-theme="retro">
<body>

<div class="container" id="main">

<big>
<big>
<h1 style="font-size:2em;font-family: auto;">
	Arabic Gurmukhi Dictionary
</h1>
</big>
</big>

<hr>

<div align="right">

<!--
///
///
///
Search
///
///
--->
<form id="searchFormpt">
<input type="text" id="tags" name="laphaza" placeholder="unicode-search" onKeyUp="alphaToNum(this.value)" onclick="keyboardAppear()" onblur="keyboardDissapear()" disabled >
</form>
<!--<input type="search" id="search" name="search" placeholder="unicode-search" onclick="keyboardAppear()" onblur="keyboardDissapear()" >-->
<!-- http://ankitpokhrel.com.np/unicode-js/

http://www.branah.com/thai
 -->

<!--
/Search-
-->

</div>
<br />
 <br />



<!-- The Word -->
<big><big>
<h1 id="heading" class="fade-in-image">
  <big><span style="color:#43C6DB">{word.data[index].attributes.MaleorPresent}
  {#if word.data[index].attributes.FemaleorPast}
                      / {word.data[index].attributes.FemaleorPast}
                      {/if}


  </span></big>
  <br />
  <small><span style="color:grey;font-size:0.5em">
  {#if word.data[index].attributes.Type}
                    ({word.data[index].attributes.Type})
  {/if}

    {#if word.data[index].attributes.Lang == 'Persian'}
                      <u>Persian</u>
    {/if}
  </span></small>
</h1></big></big>
<br />


 <!-- Main Sam Arth Words -->
 <div class="panel panel-default">
  <div class="twordspt panel-body">


<p id="desc" style="color:red" class="fade-in-image">
 {word.data[index].attributes.definition}



							 </p>
							   </div>
							</div>
							 <br /><br />
                <br />

  <p>

   <span on:click={()=>indexIs(-1)} style="opacity:0.1;cursor:pointer;">Prev  -</span>





                    <span class="next_btns">
                    {#if index >= 2}
                       <a style="opacity:0.4;color:#996666" on:click={()=>indexIs(-2)}>{prevWord1},</a>
                     {/if}
                     </span>



                    <span class="next_btns" style='display:inline-block;text-align:center;'>
                     {#if index >= 1}
                      	<a style='color:#996666' on:click={()=>indexIs(-1)}>{prevWord2},</a>
                      {/if}</span>


                      <span class="next_btns" style='display:inline-block;color:#666666;text-align:center;'><u>{word.data[index].attributes.MaleorPresent}</u>,</span>


                    <span class="next_btns" style='display:inline-block;padding-left:15px;padding-right:5px;text-align:center;'>

                    <a on:click={()=>indexIs(1)}>{nextWord0},</a></span>

                    <span style="opacity:0.4;" class="next_btns"><a on:click={()=>indexIs(1)}>{nextWord1}</a></span>,

                    <!--<a href='index.php?laphaza=ਰਾਈ'></a>,

                    <a href='index.php?laphaza=ਰਾਹ'></a>-->
        <span style="opacity:0.1;cursor: pointer;" on:click={()=>indexIs(1)}>- Next</span>
 </p>


 <!-- Punjabi Keyboard-->
 <div class="keyboard" id="keyboardContainer">
 <img src="keyboard.jpg" alt="Punjabi Unicode Keys Keyboard"/>
 </div>
<br><br><br>
 </div>

</body>
</html>


<style>
body {
  padding: 30px;
  padding-left: 200px;

  background-image: url(https://live.staticflickr.com/2388/2386572246_cc73606d2e.jpg);
    background-size: cover;
    backdrop-filter: blur(3px);
    font-size: 2em;
}

.twordspt{
  font-size:1.5em;
}

.next_btns {
  max-width:175px;
  text-align: center;
  cursor: pointer;
}

#keyboardContainer{
  padding:5px;
  padding-right:1px;
  background-color:red;
  visibility:hidden;
}

.keyboard{
  position:fixed;
  bottom:0px;
  right:10px;
  opacity:0.9;
}

.keyboard img{
  width:99%;
  max-width:800px;
}

a {
  cursor:hand;
}

/* Fade in */
.fade-in-image {
  animation: fadeIn 5s;
  -webkit-animation: fadeIn 5s;
  -moz-animation: fadeIn 5s;
  -o-animation: fadeIn 5s;
  -ms-animation: fadeIn 5s;
}

@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

@-moz-keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

@-webkit-keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

@-o-keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

@-ms-keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}
/* fade in */

</style>
