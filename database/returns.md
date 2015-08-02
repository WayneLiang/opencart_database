## Returns

<a name='return'/>
### return
- return_id:int(11)
- order_id:int(11)
- product_id:int(11)
- customer_id:int(11)
- firstname:varchar(32)
- lastname:varchar(32)
- email:varchar(96)
- telephone:varchar(32)
- product:varchar(255)
- model:varchar(64)
- quantity:int(4)
- opened:tinyint(1)
- return_reason_id:int(11)
- return_action_id:int(11)
- return_status_id:int(11)
- comment:text
- date_ordered:date
- date_added:datetime
- date_modified:datetime

<a name='return_action'/>
### return_action
- return_action_id:int(11)
- language_id:int(11)
- name:varchar(64)

<a name='return_history'/>
### return_history
- return_history_id:int(11)
- return_id:int(11)
- return_status_id:int(11)
- notify:tinyint(1)
- comment:text
- date_added:datetime


<a name='return_reason'/>
### return_reason
- return_reason_id:int(11)
- language_id:int(11)
- name:varchar(128)

<a name='return_status'/>
### return_status
- return_status_id:int(11)
- language_id:int(11)
- name:varchar(32)
