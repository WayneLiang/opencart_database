## Products
<a name='attribute'/>
### attribute
- attribute_id:int(11)
- attribute_group_id:int(11)
- sort_order:int(3)

<a name='attribute_description'/>
### attribute_description
- attribute_id:int(11)
- language_id:int(11)
- name:varchar(64)

<a name='attribute_group'/>
### attribute_group
- attribute_group_id:int(11)
- sort_order:int(3)

<a name='attribute_group_description'/>
### attribute_group_description
- attribute_group_id:int(11)
- language_id:int(11)
- name:varchar(64)

<a name='category'/>
### category
- category_id:int(11)
- image:varchar(255)
- paren_id:int(11)
- top:tinyint(1)
- column:int(3)
- sort_order:int(3)
- status:tinyint(1)
- date_added:datetime
- date_modified:datetime

<a name='category_description'/>
### category_description
- category_id:int(11)
- language_id:int(11)
- name:varchar(255)
- description:text
- meta_title:varchar(255)
- meta_description:varchar(255)
- meta_keyword:varchar(255)

<a name='category_to_layout'/>
### category_to_layout
- category_id:int(11)
- store_id:int(11)
- layout_id:int(11)

<a name='category_to_store'/>
### category_to_store
- category_id:int(11)
- store_id:int(11)

<a name='download'/>
### download
- download_id:int(11)
- filename:varchar(128)
- mask:varchar(128)
- date_added:datetime

<a name='download_description'/>
### download_description
- download_id:int(11)
- language_id:int(11)
- name:varchar(64)

<a name='manufacturer'/>
### manufacturer
- name:varchar(64)
- image:varchar(255)
- sort_order:int(3)

<a name='manufacturer_to_store'/>
### manufacturer_to_store
- manufacturer_id:int(11)
- store_id:int(11)

<a name='option'/>
### option
- option_id:int(11)
- type:varchar(32)
- sort_order:int(3)

<a name='option_description'/>
### option_description
- option_id:int(11)
- language_id:int(11)
- name:varchar(128)

<a name='option_value'/>
### option_value
- option_value_id:int(11)
- option_id:int(11)
- image:varchar(255)
- sort_order:int(3) 
 
<a name='option_value_description'/>
### option_value_description
- option_value_id:int(11)
- language_id:int(11)
- option_id:int(11)
- name:varchar(128)
 
<a name='product'/>
### product
- product_id:int(11)
- model:varchar(64)
- sku:varchar(64)
- upc:varchar(12)
- ean:varchar(14)
- jan:varchar(13)
- isbn:varchar(17)
- mpn:varchar(64)
- location:varchar(128)
- quantity:int(4)
- stock_status_id:int(11)
- image:varchar(255)
- manufacturer_id:int(11)
- shipping:tinyint(1)
- price:decimal(15,4)
- points:int(8)
- tax_class_id:int(11)
- date_available:date
- weight:decimal(15,8)
- weight_class_id:int(11)
- length:decimal(15,8)
- width:decimal(15,8)
- height:decimal(15,8)
- length_class_id:int(11)
- subtract:tinyint(1)
- minimum:int(11)
- sort_order:int(11)
- status:tinyint(1)
- viewed:int(5)
- date_added:datetime
- date_modified:datetime

<a name='product_attribute'/>
### product_attribute
- product_id:int(11)
- attribute_id:int(11)
- language_id:int(11)
- text:text

<a name='product_description'/>
### product_description
- product_id:int(11)
- language_id:int(11)
- name:varchar(255)
- description:text
- tag:text
- meta_title:varchar(255)
- meta_description:varchar(255)
- meta_keyword:varchar(255)

<a name='product_discount'/>
### product_discount
- product_discount_id:int(11)
- product_id:int(11)
- priority:int(5)
- price:decimal(15,4)
- date_start:date
- date_end:date

<a name='product_image'/>
### product_image
- product_image_id:int(11)
- product_id:int(11)
- image:varchar(255)
- sort_order:int(3)

<a name='product_option'/>
### product_option
- product_option_id:int(11)
- product_id:int(11)
- option_id:int(11)
- value:text
- required:tinyint(1)

<a name='product_option_value'/>
### product_option_value
- product_option_value_id:int(11)
- product_option_id:int(11)
- product_id:int(11)
- option_id:int(11)
- option_value_id:int(11)
- quantity:int(3)
- subtract:tinyint(1)
- price:decimal(15,4)
- price_prefix:varchar(1)
- points:int(8)
- points_prefix:varchar(1)
- weight:decimal(15,8)
- weight_prefix:varchar(1)

<a name='product_related'/>
### product_related
- product_id:int(11)
- related_id:int(11)

<a name='product_reward'/>
### product_reward
- product_reward_id:int(11)
- product_id|int(11)
- customer_group_id:int(11)
- points:int(8)

<a name='product_special'/>
### product_special
- product_special_id:int(11)
- product_id:int(11)
- customer_group_id:int(11)
- priority:int(5)
- price:decimal(15,4)
- date_start:date
- date_end:date

<a name='product_to_category'/>
### product_to_category
- product_id:int(11)
- category_id:int(11)

<a name='product_to_download'/>
### product_to_download
- product_id:int(11)
- download_id:int(11)

<a name='product_to_layout'/>
### product_to_layout
- product_id:int(11)
- store_id:int(11)
- layout_id:int(11)

<a name='product_to_store'/>
### product_to_store
- product_id:int(11)
- store_id:int(11)

<a name='review'/>
### review
- review_id:int(11)
- product_id:int(11)
- customer_id:int(11)
- author:varchar(64)
- text:text
- - rating:int(1)
- status:tinyint(1)
- date_added:datetime
- date_modified:datetime

<a name='stock_status'/>
### stock_status
- stock_status_id:int(11)
- language_id:int(11)
- name:varchar(32)

### filter
- filter_id:int(11)
- - filter_group_id:int(11)
- sort_order:int(3)

### filter_description
- filter_id:int(11)
- language_id:int(11)
- filter_group_id:int(11)
- name:varchar(64)

### filter_group
- filter_group_id:int(11)
- sort_order:int(3)

### filter_group_description
- filter_group_id:int(11)
- language_id:int(11)
- name:varchar(64)