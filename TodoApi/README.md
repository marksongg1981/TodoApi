# WeatherForecastControllerApi
 Asp.net Api
 チュートリアル: ASP.NET Core で Web API を作成する
 
https://docs.microsoft.com/ja-jp/aspnet使用前面的说明添加 Microsoft.EntityFrameworkCore.InMemory NuGet 包。/core/tutorials/first-web-api?view=aspnetcore-3.1&tabs=visual-studio
【Microsoft.EntityFrameworkCore.InMemory NuGet 包】必须要安装


* * *

Ctrl キーを押しながら F5 キーを押して、アプリを実行します。 Visual Studio でブラウザーが起動し、https://localservices.AddDbContext<TodoContext>(opt =>
               opt.UseInMemoryDatabase("TodoList"));host:<port>/WeatherForecast にアクセスします。ここで、<port> はランダムに選択されたポート番号になります。
   [UseInMemoryDatabase]  使用以方便时，是在内存中创建数据库，iis停止后，数据不再持久化


**Postman のインストール**
このチュートリアルでは、Postman を使用して Web API をテストします。
Postman をインストールします。
Web アプリを起動します。
Postman を起動します。
[SSL 証明書の確認] を無効にします。
[ファイル] > [設定] ( [全般] タブ) で、 [SSL 証明書の確認] を無効にします。
 警告

コントローラーをテストした後、SSL 証明書の検証を再度有効にします。

Postman を使用した PostTodoItem のテスト
新しい要求を作成します。
HTTP メソッドを POST に設定します。
[Body] タブを選択します。
[raw] ラジオ ボタンを選択します。
型を [JSON (application/json)] に設定します。
要求本文に、To Do アイテムの JSON を入力します。
JSON

コピー
{
  "name":"walk dog",
  "isComplete":true
}
[Send] を選択します。

**[JOSN(application/json)]必须要选择。**
