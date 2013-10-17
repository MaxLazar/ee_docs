
#### Entry Form with using the {custom_fields} loop
	{exp:channel:form channel="products" return="form_template/ENTRY_ID" entry_id="{segment_2}"}
		...
		{custom_fields}
					<label for="{field_name}">{if required}* {/if}{field_label}</label>
					{if mx_select_plus}
						{field:mx_select_plus_field_name}
					{/if}
		{/custom_fields}
		...
	{/exp:channel:form}

#### Entry Form without using the {custom_fields} loop

	{exp:channel:form channel="products" return="form_template/ENTRY_ID" entry_id="{segment_2}"}
		...
		{custom_fields}
					<label for="{field_name}">{if required}* {/if}{field_label}</label>
					{if mx_select_plus}
						{field:mx_select_plus_field_name}
					{/if}
		{/custom_fields}
		...
	{/exp:channel:form}