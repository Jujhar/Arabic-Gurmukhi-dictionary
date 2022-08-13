<script>
let index = 0;
$: place = index;

let word = {"data":[{"id":1,"attributes":{"definition":"to please","createdAt":"2022-05-16T01:01:40.251Z","updatedAt":"2022-08-13T17:06:55.797Z","MaleorPresent":"ਯੁਜਬੋ","FemaleorPast":"ਆਜ਼ਬਾ","Type":"Past / Present","DateAdded":"2022-06-01T07:00:00.000Z","Lang":null,"source":"https://arabic.fi/words/1049","pronunciation":"https://esanna.se/arabic/audio/1135.mp3","archive":false}},{"id":2,"attributes":{"definition":"be amazed","createdAt":"2022-05-16T01:11:51.629Z","updatedAt":"2022-08-13T17:04:39.024Z","MaleorPresent":"ਤਾਜ਼ਾਬਾ","FemaleorPast":"ਯਾਤਾਜ਼ਾਬੂ","Type":"Past / Present","DateAdded":"2022-06-01T07:00:00.000Z","Lang":null,"source":"https://arabic.fi/words/2258","pronunciation":"https://esanna.se/arabic/audio/2498.mp3","archive":false}},{"id":3,"attributes":{"definition":"amazing/spectacular","createdAt":"2022-05-16T01:15:40.897Z","updatedAt":"2022-08-13T17:06:48.635Z","MaleorPresent":"ਮੁਦਿਲ","FemaleorPast":"ਮੁਦਿਲੋਨ","Type":"Singular / Plural","DateAdded":"2022-06-01T07:00:00.000Z","Lang":null,"source":"https://arabic.fi/words/733","pronunciation":"https://esanna.se/arabic/audio/2519.mp3","archive":false}},{"id":4,"attributes":{"definition":"reverence / jaleel - majesty","createdAt":"2022-05-22T23:59:27.468Z","updatedAt":"2022-08-13T17:03:55.538Z","MaleorPresent":"ਅਜਿਾਲਾ","FemaleorPast":"ਜਲੀਲ","Type":"Male / Female","DateAdded":"2022-06-01T07:00:00.000Z","Lang":null,"source":"https://arabic.fi/words/2623","pronunciation":"https://esanna.se/arabic/audio/4124.mp3","archive":false}},{"id":5,"attributes":{"definition":"sacred","createdAt":"2022-05-23T00:04:02.554Z","updatedAt":"2022-08-13T17:06:39.974Z","MaleorPresent":"ਮੁਕਾਦਿਸ","FemaleorPast":"ਮੁਕਾਦਿਸੋਂਣ","Type":"Male / Female","DateAdded":"2022-06-01T07:00:00.000Z","Lang":null,"source":"https://arabic.fi/words/3882","pronunciation":"https://esanna.se/arabic/audio/1034.mp3","archive":false}},{"id":8,"attributes":{"definition":"food / nourishment","createdAt":"2022-06-02T17:35:46.550Z","updatedAt":"2022-08-13T17:04:48.874Z","MaleorPresent":"ਤਾਮ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":"","pronunciation":"https://esanna.se/arabic/audio/23.mp3","archive":false}},{"id":9,"attributes":{"definition":"diet / nutrition","createdAt":"2022-06-02T17:36:57.808Z","updatedAt":"2022-08-13T17:07:09.346Z","MaleorPresent":"ਰਿਦਾਓਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":"","pronunciation":"","archive":false}},{"id":11,"attributes":{"definition":"separate, detach, disconnect, break, dismiss","createdAt":"2022-06-02T18:22:11.950Z","updatedAt":"2022-08-13T17:06:27.283Z","MaleorPresent":"ਫਸਲੁਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":12,"attributes":{"definition":"enthusiasm, intense interest, heartiness","createdAt":"2022-06-02T18:23:23.819Z","updatedAt":"2022-08-13T17:07:55.945Z","MaleorPresent":"ਹੁਮਾਸ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":13,"attributes":{"definition":"fuel","createdAt":"2022-06-02T18:25:43.270Z","updatedAt":"2022-08-13T17:07:29.458Z","MaleorPresent":"ਵਾਕੋਡੂਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":14,"attributes":{"definition":"no","createdAt":"2022-06-02T18:29:39.341Z","updatedAt":"2022-08-13T17:07:21.730Z","MaleorPresent":"ਲਾ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":15,"attributes":{"definition":"good, welfare-giving, benevolent, charitable,","createdAt":"2022-06-02T18:33:53.992Z","updatedAt":"2022-08-13T17:04:17.924Z","MaleorPresent":"ਕਾਈਰੁਨ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":16,"attributes":{"definition":"clean","createdAt":"2022-06-02T18:38:00.313Z","updatedAt":"2022-08-13T17:05:07.312Z","MaleorPresent":"ਨਾਜ਼ੀਫ","FemaleorPast":"ਨੁਜ਼ਾਫਾਤ","Type":"Singular / Plural","DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":17,"attributes":{"definition":"put, set, position, lay, design","createdAt":"2022-06-02T18:40:41.970Z","updatedAt":"2022-08-13T17:07:36.860Z","MaleorPresent":"ਵਾਡਾ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":18,"attributes":{"definition":"work, action, business, job, labor","createdAt":"2022-06-02T18:41:45.526Z","updatedAt":"2022-08-13T17:04:10.227Z","MaleorPresent":"ਆਮੁਲਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":19,"attributes":{"definition":"request, demand, order, seek, require","createdAt":"2022-06-02T18:42:50.532Z","updatedAt":"2022-08-13T17:04:57.143Z","MaleorPresent":"ਤਾਲਿਬ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":20,"attributes":{"definition":"task, mission, job, function, assignment","createdAt":"2022-06-02T18:43:43.227Z","updatedAt":"2022-08-13T17:26:31.719Z","MaleorPresent":"ਮੋਹਿਮ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}},{"id":21,"attributes":{"definition":"function, job, position, office, service","createdAt":"2022-06-02T18:44:55.981Z","updatedAt":"2022-08-13T17:07:48.779Z","MaleorPresent":"ਵਾਬੀਫਾਤਣ","FemaleorPast":null,"Type":null,"DateAdded":"2022-06-02T07:00:00.000Z","Lang":"Arabic","source":null,"pronunciation":null,"archive":false}}],"meta":{"pagination":{"page":1,"pageSize":25,"pageCount":1,"total":18}}}
;//http://localhost:1337/api/words?filters[archive][$eq]=false

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

function indexIs(i) {

  // bugfix - reload audio elment to match updated src
  if (word.data[index].attributes.pronunciation) {
    document.getElementById("aud").load();
  }

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

  &nbsp;
  {#if word.data[index].attributes.pronunciation}
  <audio id="aud" controls style="display: inline;">
      <source src={word.data[index].attributes.pronunciation} type="audio/mpeg">
      Your browser does not support the audio element.
  </audio>
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
{#if word.data[index].attributes.source}
  <a href={word.data[index].attributes.source}
     style="font-size: 0.3em; color: #7e7a7a"
     target="_blank">
    [{word.data[index].attributes.source}]
  </a>
{/if}

							   </div>
							</div>
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
<br>
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
