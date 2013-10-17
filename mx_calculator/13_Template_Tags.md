### {exp:mx_calc}
you can used it as single tag

`{exp:mx_calc expression="-4(15/42)^23*(4-sqrt(16))-15"} `

or as tag pair

	{exp:mx_calc expression="-4(15/42)^23*(4-sqrt(16))-15"}
		Cost  = {calc_result} 	
	{/exp:mx_calc} 

### Parameters

`expression="-4(15/42)^23*(4-sqrt(16))-15"`  	**required**


### Avalible functions: 

#### average
	{exp:mx_calc expression="average(4, 8, 15, 16, 23, 42)"} 

#### max
	{exp:mx_calc expression="max(4, 8, 15, 16, 23, 42)"} 

#### min
	{exp:mx_calc expression="min(4, 8, 15, 16, (3*3+8+2*3), 42)"} 

#### mod
	{exp:mx_calc expression="mod(4, 15)"} 

#### power
	{exp:mx_calc expression="power(4,2)"} 

#### round
	{exp:mx_calc expression="round(((4*5/16)/15),2)"} 

#### sum
	{exp:mx_calc expression="sum(4, 8, 15, 16, 23, 42)"} 

#### ceil
	{exp:mx_calc expression="ceil((4*5/16) / 15)"} 

#### pi
	{exp:mx_calc expression="pi()"} 

#### sqrt
	{exp:mx_calc expression="-4(15/42)^23*(4-sqrt(16))-15"} 

#### sin
	{exp:mx_calc expression="-4(15/42)^23*(4-sin(16))-15"} 

### Other functions

**sinh
arcsin
asin
arcsinh
asinh
cos
cosh
arccos
acos
arccosh
acosh
tan
tanh
arctan
atan
arctanh
atanh
abs 
ln
log**

### Single Variables

	{calc_result}
The calculation result