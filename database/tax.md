## Tax

<a name='tax_class'/>
### tax_class
- tax_class_id:int(11)
- title:varchar(32)
- description:varchar(255)
- date_added:datetime
- date_modified:datetime

<a name='tax_rate'/>
### tax_rate
- tax_rate_id:int(11)
- geo_zone_id:int(11)
- name:varchar(32)
- rate:decimal(15,4)
- type:char(1)
- date_added:datetime
- date_modified:datetime

<a name='tax_rate_to_customer_group'/>
### tax_rate_to_customer_group
- tax_rate_id:int(11)
- customer_group_id:int(11)

<a name='tax_rule'/>
### tax_rule
- tax_rule_id:int(11)
- tax_class_id:int(11)
- tax_rate_id:int(11)
- based:varchar(10)
- priority:int(5)