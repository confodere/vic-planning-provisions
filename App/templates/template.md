{% for name, sub in subdivisions.items() -%}
# {{ name }}
{% for section in sub %}
{% if section[0] is not none %}## {{section[0]}}{% endif %}
{% for  item in section[1] %}{{ item }}
{%- endfor %}
{% endfor %}
{% endfor %}