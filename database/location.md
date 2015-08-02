##Location
<a name='location'/>
### location
- location_id:nt(11)
- name:varchar(32)
- address:text
- telephone:varchar(32)
- fax:varchar(32)
- geocode:varchar(32)
- image:varchar(255)
- open:text
- comment:text

<a name='address'/>
### address
- address_id:int(11)
- customer_id:int(11)
- firstname:varchar(32)
- lastname:varchar(32)
- company:varchar(40)
- address_1:varchar(128)
- address_2:varchar(128)
- city:varchar(128)
- postcode:varchar(10)
- country_id:int(11)
- zone_id:int(11)
- custom_field:text

<a name='country'/>
### country
- country_id:int(11)
- name:varchar(128)
- iso_code_2:varchar(2)
- iso_code_3:varchar(3)
- address_format:text
- postcode_required:tinyint(1)
- status:tinyint(1)

<a name='currency'/>
### currency
- currency_id:int(11)
- title:varchar(32)
- code:varchar(3)
- symbol_left:varchar(12)
- symbol_right:varchar(12)
- decimal_place:char(1)
- value:float(15,8)
- status:tinyint(1)
- date_modified:datetime

<a name='geo_zone'/>
### geo_zone
- geo_zone_id:int(11)
- name:varchar(32)
- description:varchar(255)
- date_modified:datetime
- date_added:datetime

<a name='language'/>
### language
- language_id:int(11)
- name:varchar(32)
- code:varchar(5)
- locale:varchar(255)
- image:varchar(64)
- directory:varchar(32)
- sort_order:int(3)
- status:tinyint(1)

<a name='zone'/>
### zone
- zone_id:int(11)
- country_id:int(11)
- name:varchar(128)
- code:varchar(32)
- status:tinyint(1)

<a name='zone_to_geo_zone'/>
### zone_to_geo_zone
- zone_to_geo_zone_id:int(11)
- country_id:int(11)
- zone_id:int(11)
- geo_zone_id:int(11)
- date_added:datetime
- date_modified:datetime
