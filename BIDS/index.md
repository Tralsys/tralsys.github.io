# BIDSソフトウェア一覧

## ArduinoLibs
[TetsuOtter/TR.BIDS.ArduinoLibs](https://github.com/TetsuOtter/TR.BIDS.ArduinoLibs)

BIDS_Serverのserial modとArduinoを通信させるために使用するライブラリです.

---
## BIDS_Server
[TetsuOtter/BIDS_Server](https://github.com/TetsuOtter/BIDS_Server)

他のマシンに情報を転送する，あるいは他のマシンから情報を取得する際に使用するソフトウェアです.  
標準で以下のmodが含まれます.
- blankmod  
  : 何もしないmodです.  デバッグ用ですが一応同梱しています.
- communication  
  : Rock_On様のcommunication.dllと同じデータ配列を送受信するライブラリです.  本modに関連する質問等は[@Tetsu_Otter](htps://twitter.com/Tetsu_Otter)までお願いします.
- serial  
  : シリアル通信にて通信を行うライブラリです.  主にArduino等と通信する場合に使用することになると思います.
- swif  
  : [SkyWay WebRTC Gateway](https://github.com/skyway/skyway-webrtc-gateway)を使用して, WebRTCを用いて通信を行うために使用するライブラリです.  2021年7月1日現在開発中につきリリースには同梱していません.
- tcpcl  
  : TCP/IPにて通信を行うライブラリです.  クライアント側を担当します.
- tcpsv  
  : TCP/IPにて通信を行うライブラリです.  サーバ側を担当します.
- testmod  
  : デバッグ用のライブラリです.  ログ出力を行います.
- udp  
  : UDP/IPにて通信を行うライブラリです.  ブロードキャストを行うため, 通信相手の指定が不要で便利です.

### Additional Mod (dgoCtrlUSB)
[TetsuOtter/TR.BIDSsvMOD.dgoCtrlUSB](https://github.com/TetsuOtter/TR.BIDSsvMOD.dgoCtrlUSB)

電車でGO! 向けのコントローラを使用するためのプラグインです.

---
## BIDSDispWeb
[Tralsys/BIDSDispWeb](https://github.com/Tralsys/BIDSDispWeb)

ブラウザを使用してBIDSの情報を表示します.  通信にはSkyWayを使用します.

---
## BIDSDispX
[Tralsys/BIDSDIspX](https://github.com/Tralsys/BIDSDispX)

Xamarin.Formsを用いて開発し, スマートフォンを含む様々なデバイスでの情報表示を実現します.  2021年7月1日現在開発中です.

---
## BIDSid_SerCon
[TetsuOtter/BIDSid_SerCon](https://github.com/TetsuOtter/BIDSid_SerCon)

BVEの入力デバイスとして動作する, Arduino等とシリアル通信にて情報共有をするプラグインです.  2021年7月1日現在開発を休止しています.

---
## BIDSSMemLib
[TetsuOtter/BIDSSMemLib](https://github.com/TetsuOtter/BIDSSMemLib)

BIDSの同一マシン内情報共有用共有メモリ空間にアクセスするためのライブラリ群です.

---
## caMon
[Tralsys/caMon](https://github.com/Tralsys/caMon)

BIDSのデータを表示するためのフレームです.  標準で組み込まれているmodの使用のほか, 追加でmodを導入することで様々な表示を実現できます.  
また, modの開発を誰もが容易にできることを目標に, 開発を行っています.

### Additional Mod (HMIDisp233)
[TetsuOtter/caMonPageMod.HMIDisp233](https://github.com/TetsuOtter/caMonPageMod.HMIDisp233)

CT様より素材提供を頂き, E233系のNo.2表示器の表示内容を実装したmodです.

### Additional Mod (TIMSDisp)
[Tralsys/TR.caMonPageMod.TIMSDisp](https://github.com/Tralsys/TR.caMonPageMod.TIMSDisp)

E233系以降のTIMS表示器風の表示を実現するmodです.  2021年7月1日現在開発中です.

### Additional Mod (Type BIDSDispWeb)
[Tralsys/TR.caMonPageMod.TypeBDispW](https://github.com/Tralsys/TR.caMonPageMod.TypeBDispW)

BIDSDispWebで実装した表示をcaMonに移植したmodです.
