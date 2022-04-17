# SignalRChat

快速上手 ASP.NET Core SignalR

## 取得 Client 端套件的方式

此專案的 JavaScript 套件是透過 LibMan (Microsoft Library Manager) 取得

```sh
dotnet tool install -g Microsoft.Web.LibraryManager.Cli
libman install @microsoft/signalr -p unpkg
```

> 補充：針對此類型的專案，其實只需要這兩個檔案就好了！
> * `wwwroot/lib/microsoft/signalr/dist/browser/signalr.min.js`
> * `wwwroot/lib/microsoft/signalr/dist/browser/signalr.min.js.map`



## 注意事項

若 Client 與 Server 位於不同的來源，則必須加入 CORS 支援