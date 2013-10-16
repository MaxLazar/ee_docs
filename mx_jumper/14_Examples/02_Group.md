	{exp:channel:entries channel="news" limit="15"}
		<h3>{title}</h3>
		
		{body}
		
		<div class="date">Posted on {entry_date format="%M %d, %Y - %h:%i %A"}</div>
		
		{exp:mx_jumper:put_group name="country_list"}{country}{/exp:mx_jumper:put_group}
	{/exp:channel:entries}

**Menu:**

	<ul>
	{exp:mx_jumper:out_group name="country_list"}
		<li>{item}</li>
	{/exp:mx_jumper:out_group}
	<ul> 