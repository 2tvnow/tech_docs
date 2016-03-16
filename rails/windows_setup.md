#### 1. 下載安裝Ruby與DevKit

(1) 前往 http://rubyinstaller.org/   
(2) 下載安裝 `Ruby 2.x.x`   
(3) 下載DevKit，注意如果是x64要用 64bits only   

將檔案解壓縮到 `C:\DevKit`，然後進入該目錄執行：

``` 
$ ruby dk.rb init 
$ ruby dk.rb install   
```

#### 2. 安裝Rails與Bundler

```
$ gem install rails
$ gem install bulder
```
 
#### 3. 建立一個Rails專案並執行

```
$ rails new rails_demo
$ cd rails_demo
$ bundle install
$ rails s
```
