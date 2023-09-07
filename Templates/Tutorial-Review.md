---
created: 2023-07-12T10:47:19-05:00
updated: 2023-09-07T09:39:00-05:00
---

## {{title}} 
> [!info] 
> - **Abstract:** {{abstractNote}} 
> - **Sources**: [online]({{uri}}) [local]({{desktopURI}}) {%- for attachment in attachments | filterby("path", "endswith",".pdf") %} [pdf](file:///{{attachment.path | replace(" ","%20")}}) {% if loop.last %}{% endif %}{%- endfor %}
> - **Cite Key:** [[@{{citekey}}]] 
> - **Programming Language**: 
> - **Software:**
 {%- if hashTags %}
> - **Tags:** {{hashTags}} 
{%- endif %}

## Annotations 
{% for annotation in annotations %}
	{% if annotation.annotatedText %}
		 {{annotation.annotatedText}}
	{% endif %}
   {% if annotation.comment %}
		{{annotation.comment}}
	{% endif %}
{% endfor %}


