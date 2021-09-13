## usersテーブル

|Column|Type|Options|
|password|string|null:false|
|email|string|null:false|
|name|string|null:false|
|profile|text|null:false|
|occupation|text|null:false|
|position|text|null:false|

# Association
-belongs_to :user
-has_many :comments

## commentsテーブル

|Column|Type|OPtions|
|text|string|null:false,foreign_key: true|
|user|references|foreign_key:true|
|prototypes|references|foreign_key:true|
# Association
-belongs_to:user
belongs_to:prototype