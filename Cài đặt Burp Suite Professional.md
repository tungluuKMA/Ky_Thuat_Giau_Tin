# Cài đặt Burp Suite Professional

## Cài đặt Burp Suite Professional

Truy cập [https://portswigger.net/burp/releases#professional](https://portswigger.net/burp/releases#professional) ,tải bản **Stable** mới nhất về và cài đặt nó 😀

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled.png?raw=true)

## Tải tài liệu 😀

Tải `BurpLoaderKeygen.jar` tại [https://github.com/h3110w0r1d-y/BurpLoaderKeygen/releases/latest](https://github.com/h3110w0r1d-y/BurpLoaderKeygen/releases/latest)

[BurpLoaderKeygen.zip](Cài%20đặt%20Burp%20Suite%20Professional/BurpLoaderKeygen.zip?raw=true)

Tải `BurpSuitePro.zip` phía dưới và giải nén ra để được `BurpSuitePro.exe`

[BurpSuitePro.zip](Cài%20đặt%20Burp%20Suite%20Professional/BurpSuitePro.zip?raw=true)

Copy `BurpLoaderKeygen.jar`  và `BurpSuitePro.exe` đến `%LOCALAPPDATA%\Programs\BurpSuitePro` hoặc `%LOCALAPPDATA%\BurpSuitePro` tuỳ theo vị trí cài đặt Burp Suite

## Crack License 😈

Tại [thư mục cài đặt](Cài%20đặt%20Burp%20Suite%20Professional.md) của Burp Suite, mở CMD:

```bash
jre\bin\java -jar BurpLoaderKeygen.jar
```

Tại Cửa sổ KeyLoader, tích chọn **Auto Run** và **Ignore Update,** custom tên **License text** nếu muốn sau đó **Run** để khởi chạy Burp Suite

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled%201.png?raw=true)

Tại cửa số nhập License, Copy License từ Burp Loader và dán vào sau đó bấm Next

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled%202.png?raw=true)

Tại cửa sổ phía sau, lựa chọn **Manual activation**

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled%203.png?raw=true)

Tại cửa sổ phía sau, copy request từ mục 2 bên **Burp Suite**, và paste tại **Activation Request** phía **Burp Loader**

Sau đó copy **Activation Response** từ **Burp Loader** và paste vào response tại mục 3 của **Burp Suite**.

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled%204.png?raw=true)

Bấm Next và kích hoạt thành công. 

Bấm Finish để kết thúc.

![Untitled](Cài%20đặt%20Burp%20Suite%20Professional/Untitled%205.png?raw=true)

## Crack lại sau khi Update

Sau khi update, chỉ cần tải lại `[BurpSuitePro.exe](Cài%20đặt%20Burp%20Suite%20Professional.md)`, sau đó ghi đè vào [thư mục cài đặt](Cài%20đặt%20Burp%20Suite%20Professional.md)