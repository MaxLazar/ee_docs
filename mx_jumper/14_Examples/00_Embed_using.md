	<html lang="en">
	<head>
	 {embed="include/.meta"}
	</head>
	<body>
	     {exp:channel:entries channel="news"}
	     {exp:mx_jumper:put name="title"}title{/exp:mx_jumper:put} 
	     ....
	     {/exp:channel:entries}
	</body>
	</html> 

**include/.meta** 

	<title>EEC.MS - {exp:mx_jumper:out name=“title”}</title> 