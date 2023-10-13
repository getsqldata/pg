qs	qs	qs
<pre>
<code>
create temp table t1 (id int);

insert into t1 values (1),(2),(3),(4),(5),(10),(11),(12);

select 
	id, 
	sum(id) over(order by id) 
from t1; 
</code>
</pre>
hrthrthth


<h3>Start with text hidden:</h3>  
<button id="light1_butt" onclick=${() => {
  document.getElementById("light1_text").hidden = document.getElementById("light1_text").hidden? false : true;
  let btext = document.getElementById("light1_butt").innerText;
  document.getElementById("light1_butt").innerText = (btext[0] == 'H')? btext.replace("Hide","Show") : btext.replace("Show","Hide");
  }
}>Show the text</button>
<div id='light1_text' hidden>
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
</div>
