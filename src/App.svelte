<script>

let index = 0;
$: place = index;

let word = {"data":[{"id":1,"attributes":{"definition":"to please","createdAt":"2022-05-16T01:01:40.251Z","updatedAt":"2022-05-16T02:10:12.283Z","MaleorPresent":"ਯੁਜਬੋ","FemaleorPast":"ਆਜ਼ਬਾ","Type":"Past / Present"}},{"id":2,"attributes":{"definition":"be amazed","createdAt":"2022-05-16T01:11:51.629Z","updatedAt":"2022-05-16T02:10:01.285Z","MaleorPresent":"ਤਾਜ਼ਾਬਾ","FemaleorPast":"ਤਾਜ਼ਾਬੂ","Type":"Past / Present"}},{"id":3,"attributes":{"definition":"amazing/spectacular","createdAt":"2022-05-16T01:15:40.897Z","updatedAt":"2022-05-16T02:10:06.824Z","MaleorPresent":"ਮੁਦਿਲ","FemaleorPast":"ਮੁਦਿਲੋਨ","Type":"Singular / Plural"}}],"meta":{"pagination":{"page":1,"pageSize":25,"pageCount":1,"total":3}}}

function indexIs(i){
  console.log('index is'+index);
  index = index+i;
  console.log('index is now'+index);
}

//prevWord0 = word[index-3];
//prevWord1 = x;
//prevWord2 = x;
let nextWord0 = word.data[index+1].attributes.MaleorPresent;
let nextWord1 = word.data[index+2].attributes.MaleorPresent;
//nextWord2 = x;
//nextWord3 = x;

console.log(word);


</script>

<html data-theme="retro">
<body>

<div class="container" id="main">

<big>
<big>
<h1 style="font-size:2em;">
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
<h1>
  <big><span style="color:#43C6DB">{word.data[index].attributes.MaleorPresent} / {word.data[index].attributes.FemaleorPast}</span></big>
  <br />
  <small><span style="color:grey;font-size:0.5em">({word.data[index].attributes.Type})</span></small>
</h1></big></big>
<br />


 <!-- Main Sam Arth Words -->
 <div class="panel panel-default">
  <div class="twordspt panel-body">

<p style="color:red">
 {word.data[index].attributes.definition}



							 </p>
							   </div>
							</div>
							 <br /><br />
                <br /><br />
                 <br /><br />

  <p>

   <span style="opacity:0.1">Prev  -</span>





										<a href='index.php?laphaza=ਰਣਵਾਸ' style='color:#996666'>,</a>
                     <span style='display:inline-block;text-align:center;'><a href='index.php?laphaza=ਰਤਨ ਜੋਤ' style='color:#996666'>,</a>


                     </span> <span style='display:inline-block;color:#666666;text-align:center;'>{word.data[index].attributes.MaleorPresent},</span>


                    <span style='display:inline-block;padding-left:15px;padding-right:5px;text-align:center;'>

                    <a on:click={()=>indexIs(1)}>{nextWord0},</a></span>

                    <a on:click={()=>indexIs(0)}>{nextWord1}</a>,

                    <a href='index.php?laphaza=ਰਾਈ'></a>,

                    <a href='index.php?laphaza=ਰਾਹ'></a>
        <span style="opacity:0.1">- Next</span>
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
}
.twordspt{
font-size:1.5em;
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
  </style>
