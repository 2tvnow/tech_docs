新增欄位 add_column(TABLE, 欄位, 型態, Options)
------------------------------------------------

命名規則: `add_欄位_to_TABLE`

例: 幫cat model新增一個欄位nick_name

執行 `$ rails g migration add_nick_name_to_cats`

修改 `add_nick_name_to_cats.rb` 如下  

```
class AddNickNameToCats < ActiveRecord::Migration
  def change
    add_column :cats, :nick_name, :string
  end
end
```

修改欄位名稱 rename_column(TABLE, 舊欄位名稱, 新欄位名稱)
----------------------------------------

命名規則: `rename_舊欄位名稱_to_新欄位名稱_of_TABLE`

例: 將cat model的nick_name改名為name
  
執行 `$ rails g migration rename_nick_name_to_name_of_cats`   

修改 `rename_nick_name_to_name_of_cats.rb` 如下

```
class RenameNickNameToNameOfCats < ActiveRecord::Migration
  def change
    rename_column  :cats, :nick_name, :name
  end
end
```

刪除欄位 remove_column(TABLE, 欄位)
----------------------------------------

命名規則: `remove_欄位_from_TABLE`

例: 移除cat model的nick_name  

執行 `$ rails g migration remove_nick_name_from_cats`   

修改 `remove_nick_name_from_cats.rb` 如下

```
class RemoveNickNameFromCats < ActiveRecord::Migration
  def change
    remove_column  :cats, :nick_name
  end
end
```

修改欄位 change_column(TABLE, 欄位, 型態, Options)
---------------------------------------------------
 
命名規則: `change_欄位_to_修改的內容_of_TABLE`

例: 將cat model的nick_name改為integer型態  

執行 `$ rails g migration change_nick_name_to_integer_type_of_cats`   

修改 `change_nick_name_to_integer_type_of_cats.rb` 如下

```
class ChangeNickNameToIntegerTypeOfCats < ActiveRecord::Migration
  def change
    change_column :cats, :nick_name, :integer
  end
end
```
