Data_mining_project

Merchants sometimes run big promotions (e.g., discounts or cash coupons) on particular dates, such as "Black Friday" or "Double 11 (Nov 11th)”, to attract potential new buyers. Unfortunately, many of these buyers are one-time deal hunters, and these promotions may have a little long-term impact on sales in the future. To alleviate this problem, merchants need to identify who can be converted into repeated buyers.


[Original Data Resources](https://tianchi.aliyun.com/competition/entrance/231576/information)

There following are some descriptions of the data files.

| Data Fields | Definition |
|-|-|
| user_id | A unique id for the shopper. |
| age_range | User' s age range: 1 for <18; 2 for [18,24]; 3 for [25,29]; 4 for [30,34]; 5 for [35,39]; 6 for [40,49]; 7 and 8 for >= 50; 0 and NULL for unknown. |
| gender | User' s gender: 0 for female, 1 for male, 2 and NULL for unknown. |
| merchant_id | A unique id for the merchant. |
| label | Value from {0, 1, -1, NULL}. ' 1' denotes ' user_id' is a repeat buyer for ' merchant_id' , while ' 0' is the opposite. ' -1' represents that ' user_id' is not a new customer of the given merchant, thus out of our prediction. However, such records may provide additional information. ' NULL' occurs only in the testing data, indicating it is a pair to predict. |
| activity_log | Set of interaction records between {user_id, merchant_id}, where each record is an action represented as ' item_id:category_id:brand_id:time_stamp:action_type' . ' #' is used to separate two neighbouring elements. Records are not sorted in any particular order. |

