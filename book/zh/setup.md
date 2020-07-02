# 安裝與設定 HonKit

安裝 HonKit 並讓它順利運作通常只需要幾分鐘的時間。

> 需要在你的電腦上使用終端機指令、Git，可能也需要對 Node.js 與 NPM 有基礎理解。

### 在電腦上安裝

##### 系統需求

安裝 HonKit 相當簡單與直觀，只需要滿足下面兩項需求：

* NodeJS (建議使用 v10.0.0 或更新的版本）
* Windows, Linux, Unix 或 macOS X

##### 使用 NPM 安裝

使用 **NPM** 或 **Yarn** 安裝 HonKit，只需要在終端機提示後簡單輸入下面的指令：

```
$ npm install honkit --save-dev
# or
$ yarn install honkit --save
```

> 由於目前 `honkit` 仍在快速開發階段，更新相對頻繁，開發者建議安裝在工作目錄而非全域環境（global），但若以過去使用 `gitbook-cli` 的經驗來看，安裝於全域才能便利的在不同目錄下產製書籍。

##### 開始一本新書

HonKit can setup a boilerplate book:

```
$ honkit init
```

If you wish to create the book into a new directory, you can do so by running `honkit init ./directory`

Preview and serve your book using:

```
$ honkit serve
```

Or build the static website using:

```
$ honkit build
```


##### Debugging

You can use the options `--log=debug` and `--debug` to get better error messages (with stack trace). For example:

```
$ honkit build ./ --log=debug --debug
```

