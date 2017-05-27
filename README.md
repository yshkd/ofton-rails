## ofton-rails

## バージョン

|key    |version |
|:-----:|:------:|
|ruby   | 2.3.1  |
|Rails  | 5.1.1  |
|bundler| 1.15.0 |
|node   | v7.0.0 |

## 開発環境構築

### Xcode,Command Line Toolsのインストール

下記コマンドを実行
```
xcode-select --install
```

### Homebrewのインストール

下記コマンドを実行
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### rbenvのインストール

下記コマンドを実行
```
brew install rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
brew install ruby-build
brew install rbenv-gemset
brew install rbenv-gem-rehash
source ~/.bash_profile
```

### ruby2.2.0のインストール
下記コマンドを実行
```
rbenv install 2.3.1
rbenv rehash #今は必要ないらしい
rbenv global 2.3.1
```
or local...

### bundlerのインストール
下記コマンドを実行
```
gem install bundler --version=1.15.0
```

### railsのインストール
下記コマンドを実行
```
gem install rails
```

### sqlite3のインストール
https://www.tutorialspoint.com/sqlite/sqlite_installation.htm

### npmのインストール

- `ndenv`を各自installしてください

```
ndenv install v7.0.0
ndenv local v7.0.0
npm install
```

Get on Rails
```
bin/bundle install --path vendor/bundle --jobs 4
bin/rails server
```

## 初期設定
### DB作成
`ofton_development` というDBを作成

### 環境変数設定
`.env.sample`をコピーして`.env`を作成

参考) http://qiita.com/closer/items/f8d8ba00ae86d7051764

今後、環境変数の追加はあります。
