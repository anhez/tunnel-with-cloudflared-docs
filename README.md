# Tunnel với Cloudflared

## Cài đặt

To download and install cloudflared:

```bash
brew install cloudflared
```

## Cấu hình
Em/Anh sẽ gửi cho mọi người file cấu hình cho từng app, sẽ có 2 file cấu hình: 
```config-[YOUR-APP-NAME].yml``` và ```xxxx-xxx-xxx-xxxx.json```

Trong file ```config-[YOUR-APP-NAME].yml``` thì mọi người cần sửa lại **port** và **đường dẫn chính xác** tới file .json trên thiết bị của mình




## Chạy

```
cloudflared tunnel --config /Users/anhez/.cloudflared/config-[YOUR-APP-NAME].yml run [YOUR-APP-NAME]
```
*Note: hãy đảm bảo sửa [YOUR-APP-NAME] và đường dẫn config khi chạy lệnh *

URL của tunnel sẽ có dạng: ```your-app-name.takinato.dev```
