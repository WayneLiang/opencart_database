## Customers
<a name='coupon'/>
### coupon
- coupon_id:int(11)
- name:varchar(128)
- code:varchar(10)
- type:cahr(1)
- discount:deciaml(15,4)
- logged:tinyint(1)
- shipping:tinyint(1)
- total:decimal(15,4)
- date_start:date
- date_end:date
- uses_total:int(11)
- uses_customer:varchar(11)
- status:tinyint(1)
- date:added:datetime

<a name='coupon_history'/>
### coupon_history
- coupon_history_id:int(11)
- - coupon_id:int(11)
- order_id:int(11)
- customer_id:int(11)
- amount:decimal(15,4)
- date_added:datetime

<a name='coupon_products'/>
### coupon_product
- coupon_product_id:int(11)
- coupon_id:int(11)
- product_id:int(11)

<a name='coupon_products'/>
### coupon_category
- coupon_id:int(11)
- category_id:int(11)

<a name='customer'/>
### customer
- customer_id:int(11)
- customer_group_id:int(11)
- store_id:int(11)
- firstname:varchar(32)
- lastname:varchar(32)
- email:varchar(96)
- telephone:varchar(32)
- fax:varchar(32)
- password:varchar(9)
- salt:varchar(9)
- cart:text
- wishlist:text
- newsletter:tinyint(1)
- address_id:int(11)
- custom_field:text
- ip:varchar(40)
- status:tinyint(1)
- approved:tinyint(1)
- safe:tinyint(1)
- token:text
- date_added:datetime

<a name='customer_group'/>
### customer_group
- customer-group_id:int(11)
- approval:int(1)
- sort_order:int(3)

<a name='customer_ip'/>
### customer_ip
- customer_ip_id:int(11)
- customer_id:int(11)
- ip:varchar(40)
- date_added:datetime

<a name='customer_activity'/>
### customer_activity
- activity_id:int(11)
- customer_id:int(11)
- key:varchar(64)
- data:text
- ip:varchar(40)
- date_added:datetime

<a name='customer_ban_ip'/>
### customer_ban_ip
- customer_ban_ip_id:int(11)
- ip:varchar(40)

<a name='customer_online'/>
### customer_online
- ip:varchar(40)
- customer_id:int(11)
- url:text
- referer:text
- date_added:datetime

<a name='customer_reward'/>
### customer_reward
- customer_reward_id:int(11)
- customer_id:int(11)
- order_id:int(11)
- description:text
- points:int(8)
- date_added:datetime

<a name='customer_transaction'/>
### customer_transaction
- customer_transaction_id:int(11)
- customer_id:int(11)
- order_id:int(11)
- description:text
- amount:decimal(15,4)
- date_added:datetime

<a name='customer_login'/>
### customer_login
- customer_login_id:int(11)
- email:varchar(96)
- ip:varchar(40)
- total:int(40)
- date_added:datetime
- date_modified:datetime

<a name='customer_history'/>
### customer_history
- customer_history_id:int(11)
- customer_id:int(11)
- comment:text
- date_added:datetime

<a name='custom_field'/>
### custom_field
- custom_field_id:int(11)
- type:varchar(32)
- value:text
- location:varchar(7)
- status:tinyint(1)
- sort_order:int(3)

<a name='custom_field_value'/>
### custom_field_value
- customer_field_value_id:int(11)
- customer_field_id:int(11)
- sort_order:int(3)

<a name='custom_field_value_description'/>
### custom_field_value_description
- custom_field_value_id:int(11)
- language_id:int(11)
- custom_field_id:int(11)
- name:varchar(128)

<a name='custom_field_description'/>
### custom_field_description
- custom_field_id:int(11)customer_field_customer_group
- language_id:int(11)
- name:varchar(128)

<a name='customer_field_customer_group'/>
### customer_field_customer_group
- custom_field_id:int(11)
- customer_group_id:int(11)
- required:tinyint(1)




