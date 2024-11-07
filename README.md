# CAN-FD_Board
MCP2518 + MCP2562FD CAN FD Busモジュール

### 特徴
- Microchip社のMCP2518とMCP2562FDを使い、必要なコンデンサ、水晶振動子をセットにしたCAN FDのモジュールです。
- SPI IFを使ってCANの送受信ができます。
- MCP2518の駆動電圧を5V(arduino向け)／3.3V(Rasperry Pi, ESP32向け)とジャンパにて切り替えることができます。
- 終端抵抗のあるなしをジャンパスイッチにて切り替えできます。
- MCP2518向けのドライバ、ライブラリにて簡単に利用できます。

### 基盤
![TopImage](/docs/CAN-FD_Board_Top_Image.png)
<!-- ![BottomImage](/docs/CAN-FD_4ch_HAT_Bottom_Image.png) -->
![TopPhoto](/docs/CAN-FD_Board_Top_Photo_01.jpg)
![BottomPhoto](/docs/CAN-FD_Board_Bottom_Photo_01.jpg)
![TopPhoto](/docs/CAN-FD_Board_Top_Photo_02.jpg)

### 基板の設定
![TopPhoto](/docs/CAN-FD_Board_Top_Image_explanation.jpg)

### 使用例
![UseCase_01](/docs/UseCase_01.jpg)
※CAN FD CombiBoard for ESP32を利用した例

### 資料
- [サポートページ](https://github.com/TLDSJPWORK/CAN-FD_Board)
- [回路図](/docs/CAN-FD_Board.pdf)
- [MCP2518データシート](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/External-CAN-FD-Controller-with-SPI-Interface-DS20006027B.pdf)
- [MCP2526FDデータシート](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/20005284A.pdf) 

- Rasperry Pi向け利用方法
  - [/boot/config.txt](examples/config.txt)
  - [/etc/systemd/network/49-can0.link](examples/49-can0.link)
  - [/home/pi/up.sh](examples/up.sh)
- [Arduinoライブラリ acan2517FD](https://github.com/pierremolinaro/acan2517FD)
- [Arduinoライブラリ acan2517](https://github.com/pierremolinaro/acan2517)

- [CAN FD CombiBoard for ESP32](https://github.com/TLDSJPWORK/ESP32_CAN-FD_CombiBoard)
