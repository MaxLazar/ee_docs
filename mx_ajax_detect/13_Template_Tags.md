### {exp:ajax_detect} ###
	{exp:ajax_detect}
	    {if ajax} 
	        special  code for ajax
	    {if:else}
	        for request without ajax
	    {/if}
	{/exp:ajax_detect} 

### Conditional Variables ###
if ajax

	{exp:ajax_detect}
	    {if ajax} 
	        special  code for ajax
	
	    {/if}
	{/exp:ajax_detect} 