# CAN-FD_Board
MCP2518 + MCP2562FD CAN FD Busモジュール

### 特徴
- Microchip社のMCP2518とMCP2562FDを使い、必要なコンデンサ、水晶振動子をセットにしたCAN FDのモジュールです。
- SPI IFを使ってCANの送受信ができます。
 -MCP2518の駆動電圧を5V(arduino向け)／3.3V(Rasperry Pi, ESP32向け)とジャンパにて切り替えることができます。
- 終端抵抗のあるなしをジャンパスイッチにて切り替えできます。
- MCP2518向けのドライバ、ライブラリにて簡単に利用できます。

### 基盤
![Top](/docs/CAN-FD_Board_Top.png)

### 使用例
準備中

### 資料
- [サポートページ](https://github.com/TLDSJPWORK/CAN-FD_Board)
- [回路図](/docs/CAN-FD_Board.pdf)
- [MCP2518データシート](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/External-CAN-FD-Controller-with-SPI-Interface-DS20006027B.pdf)
- [MCP2526FDデータシート](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/20005284A.pdf) 

- Rasperry Pi向け利用方法
  - [/boot/config.txt](exsamples/config.txt)
  - [/etc/systemd/network/49-can0.link](exsamples/49-can0.link)
  - [/etc/systemd/network/49-can1.link](exsamples/49-can1.link)
  - [/home/pi/up.sh](exsamples/up.sh)
- [Arduinoライブラリ acan2517FD](https://github.com/pierremolinaro/acan2517FD)
- [Arduinoライブラリ acan2517](https://github.com/pierremolinaro/acan2517)
