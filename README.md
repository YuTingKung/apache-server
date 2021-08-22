# apache-server
Apache-server doc

## 基本安裝

[下載安裝參考資料](https://dotblogs.com.tw/raylee/2019/03/06/181317)

[安裝啟動停止指令參考](https://codertw.com/%E4%BC%BA%E6%9C%8D%E5%99%A8/379261/)

1. 下載 httpd-2.4.48.tar
2. 安裝伺服器
3. Apache 的配置文件路徑(改port和起始文件): `D:\Apache Software Foundation\Apache24\conf\httpd.conf`

## 相關指令

1) 安裝apache服務

`httpd.exe -k install`

2) 指定要安裝的服務的名稱（適用於電腦上有幾個不同的Apache服務設施）

`httpd.exe -k install -n "MyServiceName"`

3) 指定服務配置檔案的路徑和名稱

`httpd.exe -k install -n "MyServiceName" -f "c:\files\my.conf"`

注：若不使用特殊引數（如httpd.exe -k install），服務名稱為Apache2.X，配置檔案為conf\httpd.conf

4) 移除一個Apache服務

`httpd.exe -k uninstall`

5) 移除特定的Apache服務

`httpd.exe -k uninstall -n "MyServiceName"`

管理Apache服務

1) 啟動已安裝的Apache服務

`httpd.exe -k start`

2) 停止已安裝的Apache服務

`httpd.exe -k stop || httpd.exe -k shutdown`

3) 重啟已安裝的Apache服務(迫使服務重讀配置檔案，適用於修改配置檔案後)

`httpd.exe -k restart`
