# OpenCart 数据字典

72## oc_address
**地址表：用于存放会员的地址信息**<br>
**主键：address_id**
- address_id:int(11)     地址ID主键（自动增长）
- customer_id:int(11)    会员的注册ID（与customer的主键关联）
- firstname:varchar(32)  名
- lastname:varchar(32)   姓
- company:varchar(40)    公司名称
- address_1:varchar(128) 街道地址
- address_2:varchar(128) 地址可随意写
- city:varchar(128)      城市
- postcode:varchar(10)   邮编
- country_id:int(11)     国家编号（关联country表的主键country_id）
- zone_id:int(11)        地区编号（关联zone表的主键zone_id）
- custom_field:text      习惯过滤

60## oc_affiliate
**分支机构表：用于存放分支机构信息**<br>
**主键：affiliate_id**
- affiliate_id:int(11)   分支机构ID主键（自动增长）
- firstname:varchar(32)  名
- lastname:varchar(32)   姓
- email:varchar(96)      邮箱
- telephone:varchar(32)  电话
- fax:varchar(32)        传真
- password:varchar(40)   密码
- salt:varchar(9)        
- company:varchar(40)    公司名称
- website:varchar(255)   网站
- address_1:varchar(128) 街道地址
- address_2:varchar(128) 地址可随意写
- city:varchar(128)      城市
- postcode:varchar(10)   邮编
- country_id:int(11)     国家编号（关联country表的主键country_id）
- zone_id:int(11)        地区编号（关联zone表的主键zone_id）
- code:varchar(64)       
- commission:decimal(4,2)
- tax:varchar(64)
- payment:varchar(6)
- cheque:varchar(100)
- paypal:varchar(64)
- bank_name:varchar(64)
- bank_branch_number:varchar(64)
- bank_swift_code:varchar(64)
- bank_account_name:varchar(64)
- bank_account_number:varchar(64)
- ip:varchar(40)
- status:tinyint(1)
- approved:tinyint(1)
- date_added:detetime

## oc_affiliate_activity
**分支机构活动表**<br>
**主键：activity_id**
- activity_id:int(11)
- affiliate_id:int(11)
- key:varchar(64)
- data:text
- ip:varchar(40)
- date_added:datetime

## oc_affiliate_login
**分支机构登录表**
**主键：affiliate_login_id**
- affiliate_login_id:int(11)
- email:varchar(96)
- ip:varchar(40)
- total:int(4)
- date_added:datetime
- date_modified:datetime

61## oc_affiliate_transaction
**分支机构交易表：分支机构的交易信息**
**主键：affiliate_transaction_id**


## oc_api

- api_id:int(11)
- username:varchar(64)
- password:text
- status:tinyint(1)
- date_added:datetime
- date_modified:datetime
  
## c_api_ip

- api_ip_id:int(11)
- api_id:int(11)
- ip:varchar(40)

## oc_api_session

- api_session_id:int(11)
- api_id:int(11)
- token:varchar(32)	
- session_id:varchar(32)	
- session_name:varchar(32)
- ip:int(11)
- date_added:datetime
- date_mofified:datetime

29## oc_attribute

- attribute_id:int(11)
- attribute_group_id:int(11)
- sort_order:int(3)


30## oc_attribute_description

- attribute_id:int(11)
- language_id:int(11)
- name:varchar(64)


31## oc_attribute_group

- attribute_group_id:int(11)	
- sort_order:int(3)	

32## oc_attribute_group_description

- attribute_group_id:int(11)
- language_id:int(11)
- name:varchar(64)

1## oc_banner

- banner_id:
- name:varchar(64)
- status:tinyint(1)

2## oc_banner_image

- banner_image_id:int(11)
- banner_id:int(11)
- link:varchar(255)
- image:varchar(255)
- sort_order:int(3)


3## oc_banner_image_description

- banner_image_id:int(11)
- language_id:int(11)
- banner_id:int(11)
- title:varchar(64)

33## oc_category

- category_id:int(11)
- image:varchar(255)
- parent_id:int(11)
- top:tinyint(1)
- column:int(3)
- sort_order:int(3)
- status:tinyint(1)
- date_added:datetime
- date_modified:datetime

34## oc_category_description

- category_id:int(11)
- language_id:int(11)
- name:varchar(255)
- description:text
- meta_title:varchar(255)
- meta_description:varchar(255)
- meta_keyword:varchar(255)


## oc_category_filter

- category_id:int(11)	
- filter_id:int(11)	

## oc_category_path

- category_id:int(11)	
- path_id:int(11)	
- level:int(11)	


35## oc_category_to_layout

- category_id:int(11)	
- store_id:int(11)	
- layout_id:int(11)	

36## oc_category_to_store

- category_id:int(11)
- store_id:int(11)


73## oc_country

- country_id:int(11)
- name:varchar(128)
- iso_code_2:varchar(2)
- iso_code_3:varchar(2)
- address_format:text
- postcode_required:tinyint(1)
- status:tinyint(1)


20## oc_coupon

- coupon_id
- name
- code
- type
- discount
- logged
- shipping
- total
- date_start
- date_end
- uses_total
- uses_customer
- status
- date_added

Customers## oc_coupon_category

-
-
-
-
-
-
-
-
-
-
-

21## oc_coupon_history

-
-
-
-
-
-
-
-
-
-
-

22## oc_coupon_product

-
-
-
-
-
-
-
-
-
-
-

74## oc_currency

-
-
-
-
-
-
-
-
-
-
-
23## oc_customer

-
-
-
-
-
-
-
-
-
-
-

Customers## oc_customer_activity

-
-
-
-
-
-
-
-
-
-
-

Customers## oc_customer_ban_ip

24## oc_customer_group

Customers## oc_customer_group_description

Customers## oc_customer_history

25## oc_customer_ip

Customers## oc_customer_login

Customers## oc_customer_online

26## oc_customer_reward

27## oc_customer_transaction

## oc_custom_field

## oc_custom_field_customer_group

## oc_custom_field_description

## oc_custom_field_value

## oc_custom_field_value_description

37## oc_download

38## oc_download_description

## oc_event

4## oc_extension

## oc_filter

## oc_filter_description

## oc_filter_group

## oc_filter_group_description

75## oc_geo_zone

5## oc_information

6## oc_information_description

7## oc_information_to_layout

8## oc_information_to_store

76## oc_language

9## oc_layout

Webstore## oc_layout_module

10## oc_layout_route

11## oc_length_class

12## oc_length_class_description

## oc_location

39## oc_manufacturer

40## oc_manufacturer_to_store

## oc_marketing

## oc_modification

## oc_module

41## oc_option

42## oc_option_description

43## oc_option_value

44## oc_option_value_description

62## oc_order
 
## oc_order_custom_field

63## oc_order_history

64## oc_order_option

65## oc_order_product

## oc_order_recurring

## oc_order_recurring_transaction

66## oc_order_status

67## oc_order_total

## oc_order_voucher

45## oc_product

46## oc_product_attribute

47## oc_product_description

48## oc_product_discount

## oc_product_filter

49## oc_product_image


50## oc_product_option

51## oc_product_option_value

## oc_product_recurring

52## oc_product_related

53## oc_product_reward

54## oc_product_special

55## oc_product_to_category

56## oc_product_to_download

57## oc_product_to_layout

58## oc_product_to_store

## oc_recurring

## oc_recurring_description

83## oc_return

84## oc_return_action

85## oc_return_history

86## oc_return_reason

87## oc_return_status

59## oc_review

13## oc_setting

28## oc_stock_status

14## oc_store

79## oc_tax_class

80## oc_tax_rate

81## oc_tax_rate_to_customer_group

90## oc_tax_rule

## oc_upload

15## oc_url_alias

16## oc_user

17## oc_user_group

68## oc_voucher

69## oc_voucher_history

70## oc_voucher_theme

71## oc_voucher_theme_description

18## oc_weight_class

19## oc_weight_class_description

77## oc_zone

78## oc_zone_to_geo_zone



