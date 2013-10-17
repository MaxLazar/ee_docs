###Primary Tag Pair

    <ul>
    {exp:channel:entries channel="demo" limit = "1"}
    {country}
    <li>{option} => {option_name}<br/></li>
    {/country}
    {/exp:channel:entries}
    </ul>


###Parameters

``sort="asc"``

The sort order can be ascending (asc) or descending(desc).

``limit="10"``
This parameter limits the number of results.
    

``backspace="10"``

Backspacing removes characters (including spaces and line breaks) from the last iteration of the loop.

``offset="1"``
This parameter offsets the display by X number of results.

``all_options``

      <ul>
      {exp:channel:entries channel="demo" limit = "1"}
      {country list = "on"}
       <li {if "{selected}"}class= "selected"{/if}>{option_name}</li>
      {/country}
      {/exp:channel:entries}
      </ul>


Return all options for field.


###Single Variables

``{option}``

The current option

``{option_name}``
You can used it If you have name for options.

``{count}``
The “count” out of the current entries being displayed. If five entries are being displayed, then for the fourth entry the {count} variable would have a value of “4”.

``{total_results}``
The total number of entries being displayed.

``{selected}``
You can used it with parameter all_options. It’s helps to indicate parameters which was chosen.

``:ol``

	{exp:channel:entries channel="demo" limit = "1"}
		{country:ol}
	{/exp:channel:entries}
Returns an ordered list

``:ul``

	{exp:channel:entries channel="demo" limit = "1"}
		{country:ul}
	{/exp:channel:entries}
Returns an unordered list
