#### 1. 安裝RVM

因為Mac內建的ruby版本很舊，而且會有sudo權限問題，所以統一使用RVM安裝Ruby

下載安裝RVM
```
$ \curl -sSL https://get.rvm.io | bash -s stable
```

安裝完如果有warning紅色字體，提示要加 `source ~/.profile` 到 `~/.bash_profile`裡面的話，打開.bash_profile
```
$ vi ~/.bash_profile
```

在檔案最後面加入一行
``` shell
# Add this line
source ~/.profile
```

退出後在terminal執行以下，讓.bash_profile修改後的內容馬上生效
```
$ source ~/.bash_profile
```

#### 2. 安裝Ruby

PS: 這邊的2.2.2也可以改成你需要的版本
```
$ rvm install 2.2.2
$ rvm 2.2.2 --default
```

#### 3. 安裝Rails與Bundler

```
$ gem install rails
$ gem install bulder
```
 
#### 4. 建立一個Rails專案並執行

```
$ rails new rails_demo
$ cd rails_demo
$ bundle install
$ rails s
```
