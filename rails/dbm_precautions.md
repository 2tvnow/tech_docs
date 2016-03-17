注意事項
-------

1. 產生model用 rails g model，但建立出來的table是複數，所以在操作 DB Migration之前先要確認schema.rb裡面自動產生的table名稱
2. 欄位名稱都底線分隔小寫
3. DB Migration操作的是TABLE，所以命名上我們統一參考TABLE的名稱而不是model，例如model`cat`的TABLE名稱為`cats`，命名時就要採用`cats`
4. 每次新增完migration要記得執行`rake db:migrate`
