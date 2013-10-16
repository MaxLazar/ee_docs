## Split a list of entries into blocks
Thanks to [Mark Croxton](http://devot-ee.com/members/profile/croxton/) for this example


        {exp:channel:entries parse="inwards" channel="my_weblog" orderby="title" sort="asc" disable="member_data|pagination|categories" dynamic="off"}
        
            {if count == "1"}
                <ul class="col-a">
            {/if}
            
            {if "{count}" == "{exp:mx_calc expression='ceil({total_results}/3)+1'}"}    
                </ul>
                <ul class="col-b">
            {/if}  
            
            {if "{count}" == "{exp:mx_calc expression='(ceil({total_results}/3)*2)+1'}"}        
                </ul>
                <ul class="col-c">
            {/if}
            
            <li>{title}</li>
            {if count == total_results}    
            </ul>
            {/if}
            
        {/exp:channel:entries} 