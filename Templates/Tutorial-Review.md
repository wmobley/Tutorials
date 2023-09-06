---
created: 2023-07-12T10:47:19-05:00
updated: 2023-09-06T12:01:06-05:00
---

last-reviewed:
---
## {{title}} 
> [!info] 
> - **Abstract:** {{abstractNote}} 
> - **Sources**: [online]({{uri}}) [local]({{desktopURI}}) {%- for attachment in attachments | filterby("path", "endswith",".pdf") %} [pdf](file:///{{attachment.path | replace(" ","%20")}}) {% if loop.last %}{% endif %}{%- endfor %}
> - **Bibliography**: {{bibliography}}
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


