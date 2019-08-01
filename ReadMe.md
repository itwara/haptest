### 调试
+ 目录
  + hap build
    <br> 生成dist/debug包 和 build 文件夹
  + hap release
    <br> 生成dist/release包
    <br> error:
    [LOG] ### App Loader ### 缺少私钥文件, 打包失败: /Users/wubin02/test/haptest/sign/release/private.pem
    需要手动生成：
    cd sign && mkdir release && openssl req -newkey rsa:2048 -nodes -keyout private.pem -x509 -days 3650 -out certificate.pem
+ usb 调试
  + npm run build && npm run server
  <br>必须先编译才能调试
