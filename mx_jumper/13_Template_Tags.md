### {exp:mx_jumper:put} ###
Put single piece of content

`{exp:mx_jumper:put name="city"}City{/exp:mx_jumper:put}` 

#### Parameters ####

`name= "cache_name"` *[required]*
The name parameter value is the tag which will be replaced with the tag content.

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:append} ###

	{exp:mx_jumper:append name="city" separator=" // "}New York{/exp:mx_jumper:append}

Insert content, specified by the tags, to the end of existing variable

#### Parameters ####

`name= "cache_name"` *[required]*
The name parameter value is the tag which will be replaced with the tag content.

`separator=";"` *[optional]*
Separate symbol for multiply values

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:prepend} ###
	{exp:mx_jumper:prepend name="city" separator=" // "}
		New York
	{/exp:mx_jumper:prepend}

Insert content, specified by the parameter, to the beginning of existing variable

#### Parameters ####

`name= "cache_name"` *[required]*
The name parameter value is the tag which will be replaced with the tag content.

`separator=";"` *[optional]*
`separator= " | "`
Separate symbol for multiply values

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:out} ###
Out single piece of content

#### Parameters ####

`name= "cache_name"`* [required]*
The name parameter value is the tag which will be replaced with the tag content.

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:out_global} ###
Global out of single variables

#### Parameters ####

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:put_groupt} ###
#### Parameters ####

`name= "cache_name"` *[required]*
The name parameter value is the tag which will be replaced with the tag content.

`random` 
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)

### {exp:mx_jumper:out_group} ###
Out the group of content:

	{exp:mx_jumper:out_global}
		{city}
		....
		{city_2}
	{/exp:mx_jumper:out_global} 

#### Parameters ####

`name= "cache_name"` *[required]*
The name parameter value is the tag which will be replaced with the tag content.

`random`
Prevent plugin tag caching (if you have multiple calls tags with identical parameters and tag data)