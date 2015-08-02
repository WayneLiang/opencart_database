##Other

<a name='api'/>
### api
- api_id:int(11)
- username:varchar(64)
- password:text
- status:tinyint(1)
- date_added:datetime
- date_modified:datetime

<a name='api_ip'/>
### api_ip
- api_ip_id:int(11)
- api_id:int(11)
- ip:varchar(40)

<a name='api_session'/>
### api_session
- api_session_id:int(11)
- api_id:int(11)
- token:varchar(32)
- session_id:varchar(32)
- session_name:varchar(32)
- ip:int(11)
- date_added:datetime
- date_modified:datetime

<a name='recurring'/>
### recurring
- recurring_id:int(11)
- price:decimal(10,4)
- frequency:enum('day', 'week', 'semi_month', 'month', 'year')
- duration:int(10) 
- cycle:int(10)
- trial_status:tinyint(4)
- trial_price:decimal(10,4)
- trial_frequency:enum('day', 'week', 'semi_month', 'month', 'year')
- trial_duration:int(10)
- trial_cycle:int(10)
- status:tinyint(4)
- sort_order:int(11)

<a name='recurring_description'/>
### recurring_description
- recurring_id:int(11)
- language_id:int(11)
- name:varchar(255)

<a name='module'/>
### module
- module_id:int(11)
- name:varchar(64)
- code:varchar(32)
- setting:text

<a name='upload'/>
### upload
- upload_id:int(11)
- name:varchar(255)
- filename:varchar(255)
- code:varchar(255)
- date_added:datetime

<a name='modification'/>
### modification
- modification_id:int(11)
- name:varchar(64)
- code:varchar(64)
- author:varchar(64)
- version:varchar(32)
- link:varchar(255)
- xml:text
- status:tinyint(1)
- date_added:datetime

<a name='marketing'/>
### marketing
- marketing_id:int(11)
- name:varchar(32)
- description:text
- code:varchar(64)
- clicks:int(5)
- date_added:datetime

