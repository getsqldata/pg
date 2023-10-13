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
