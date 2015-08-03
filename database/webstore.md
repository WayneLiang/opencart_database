## Webstore
<a name='banner'/>
### banner
- banner_id:int(11)
- name:varchar(64)
- status:tinyint(1)

<a name='banner_image'/>
### banner_image
- banner_image_id:int(11)
- banner_id:int(11)
- link:varchar(255)
- image:varchar(255)
- sort_order:int(3)

<a name='banner_image_description'/>
### banner_image_description
- banner_image_id:int(11)
- language_id:int(11)
- banner_id:int(11)
- title:varchar(64)

<a name='extension'/>
### extension
- extension_id:int(11)
- type:varchar(32)
- code:varchar(32)

<a name='information'/>
### information
- information_id:int(11)
- bottom:int(1)
- sort_order:int(3)
- status:tinyint(1)

<a name='information_description'/>
### information_description
- information_id:int(11)
- language_id:int(11)
- title:varchar(64)
- description:text
- meta_title:varchar(255)
- meta_description:carchar(255)
- meta_keyword:varchar(255)

<a name='information_to_layout'/>
### information_to_layout
- information_id:int(11)
- store_id:int(11)
- layout_id:int(11)

<a name='information_to_store'/>
### information_to_store
- information_id:int(11)
- store_id:int(11)

<a name='layout'/>
### layout
- layout_id:int(11)
- name:varchar(64)

<a name='layout_route'/>
### layout_route
- layout_route_id:int(11)
- layout_id:int(11)
- store_id:int(11)
- route:varchar(255)

<a name='layout_module'/>
### layout_module
- layout_module_id:int(11)
- layout_id:int(11)
- code:varchar(64)
- position:varchar(14)
- sort_order:int(3)


<a name='length_class'/>
### length_class
- length_class_id:int(11)
- value:decimal(15,8)

<a name='length_class_description'/>
### length_class_description
- length_class_id:int(11)
- language_id:int(11)

<a name='weight_class'/>
### weight_class
- weight_class_id:int(11)
- value:decimal(15,8)

<a name='weight_class_description'/>
### weight_class_description
- weight_class_id:int(11)
- language_id:int(11)
- title:varchar(32)
- unit:varchar(4)

<a name='setting'/>
### setting
- setting_id:int(11)
- store_id:int(11)
- code:varchar(32)
- key:varchar(64)
- value:text
- serialized:tinyint(1)

<a name='store'/>
### store
- store_id:int(11)
- name:varchar(64)
- url:varchar(255)
- ssl:varchar(255)

<a name='url_alias'/>
### url_alias
- url_alias_id:int(11)
- query:varchar(255)
- keyword:varchar(255)

<a name='user'/>
### user
- user_id:int(11)
- user_group_id:int(11)
- username:varchar(20)
- password:varchar(40)
- sait:varchar(9)
- firstname:varchar(32)
- lastname:varchar(32)
- email:varchar(96)
- image:varchar(255)
- code:varchar(40)
- ip:varchar(40)
- status:tinyint(1)
- date_added:datetime

<a name='user_group'/>
### user_group
- user_group_id:int(11)
- name:varchar(64)
- permission:text



