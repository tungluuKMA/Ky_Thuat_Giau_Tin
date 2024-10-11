# Cài cacert Android

### Cài đặt openssl (Windows)

```bash
winget install openssl
K chạy dc thì xem https://vietnix.vn/openssl-la-gi/
```

### Sử dụng openssl để convert cacert.der (CA Certificate của Burp Suite) thành cacert.pem

```bash
openssl x509 -inform der -in cacert.der -out cacert.pem
```

### Đổi tên file **cacert.pem** vừa tạo thành **9a5ba575.0**

```bash
openssl x509 -inform PEM -subject_hash_old -in cacert.pem
```

![name-of-cert-file.png](Cài%20cacert%20Android/name-of-cert-file.png?raw=true)

### Chạy emulator với option -writable-system

Lấy thông tin danh sách emulator

```bash
%USERPROFILE%\AppData\Local\Android\Sdk\emulator\emulator.exe -list-avds
```

![Untitled](Cài%20cacert%20Android/Untitled.png?raw=true)

Chạy emulator bằng option -writable-system với tên thiết bị được lấy từ lệnh trên

```bash
%USERPROFILE%\AppData\Local\Android\Sdk\emulator\emulator.exe -writable-system -avd Pixel_5(device's name)
```

### Remount /system

```bash
adb root
adb shell avbctl disable-verification
adb disable-verity
adb reboot
Sau khi AVD khởi động lại thì chạy lần lượt các lệnh sau:
adb root
adb remount
```

### Push **9a5ba575.0 vào thư mục cacerts**

```bash
adb push 9a5ba575.0 /system/etc/security/cacerts/
```

```bash
adb shell chmod 644 /system/etc/security/cacerts/9a5ba575.0
```

### Kiểm tra System Trusted Credentials

![Untitled](Cài%20cacert%20Android/Untitled%201.png?raw=true)