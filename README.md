# Laravel 8 透過使用者介面查看使用者活動

引入 haruncpi 的 laravel-user-activity 套件來擴增透過使用者介面查看使用者活動，幫助使用美觀，響應迅速且易於使用的使用者介面輕鬆地查看應用程式使用者活動。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 執行安裝 Laravel Mix 引用的依賴項目，並執行所有 Mix 任務。
```sh
$ npm install && npm run dev
```
> 為兼容套件 Laravel 使用者模型，使用者模型同時建立一份在放在 `app` 目錄下
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/register` 來進行註冊。
- 完成註冊後，可以經由 `/login` 來進行登入。
- 完成登入後，可以經由 `/user/activity` 來進行查看使用者活動。

----

## 畫面截圖
![](https://i.imgur.com/X6eKGEu.png)
> 查看使用者登入帳號及存取類型之紀錄
