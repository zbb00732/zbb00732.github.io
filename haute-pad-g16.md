title: 'HautePad G16'
permalink: /haute-pad-g16

## ファームウェアのWebマニュアル

- [GP2040-CE](https://gp2040-ce.info/)

## 互換性切り替え

接続時に以下のボタンを押しておくことで互換性を切り替えることができる。

この設定は接続を解除しても記憶される。

| 入力 | モード |
| --- | --- |
| B | Windows / Steam |
| A | Switch |
| X | PS3 / Direct Input |
| Y | PS4 |
| RT | キーボード |

## 方向キー設定

接続後にボタンコンビネーション入力で方向キーの設定を変更できる。

この設定は接続を解除しても記憶される。

| 入力 | モード |
| --- | --- |
| Back + Start + ↓ | D-Pad |
| Back + Start + ← | Lスティック |
| Back + Start + → | Rスティック |

## SOCD設定

接続後にボタンコンビネーション入力で方向キー同時入力の挙動を設定できる。

この設定は接続を解除しても記憶される。

| 入力 | モード |
| --- | --- |
| Home + Start + ↑ | 上優先 |
| Home + Start + ↓ | ニュートラル |
| Home + Start + ← | 最終入力優先 |

## 連射設定

接続後にTURBOボタンを押しながらボタン入力することで連射を設定できる。

同じ操作を繰り返せば設定は解除される。

## Web Config

接続時にStartボタンを押しておくことで設定ユーティリティを起動する。ユーティリティへはWebブラウザからIPv4アドレス192.168.7.1でアクセスできる。

## LED

| 入力 | モード |
| --- | --- |
| Back + Start + X | 次のアニメーション |
| Back + Start + A | 前のアニメーション |
| Back + Start + Y | 明度アップ |
| Back + Start + B | 明度ダウン |
| Back + Start + RB | LEDパラメータアップ |
| Back + Start + RT | LEDパラメータダウン |
| Back + Start + LB | 押下時パラメータアップ |
| Back + Start + LT | 押下時パラメータダウン |

## ファームウェアアップデート

1. [サポートページ](https://haute42.com/supports/)から最新Ver.の[GitHubページ](https://github.com/OpenStickCommunity/GP2040-CE/releases)へ飛ぶ
2. `flash_nuke.uf2`をダウンロードする
3. `GP2040-CE_0.X.X_Haute42.uf2`をダウンロードする
4. Startボタンを押しながらコントローラを接続する
5. Webブラウザで[192.168.7.1](http://192.168.7.1/)へアクセスする
6. `Reboot`ボタンから`Bootsel/USB`モードを起動する
7. PCにリムーバブルドライブとして`RPI-RP2`が接続される
8. `RPI-RP2`に`flash_nuke.uf2`をドラッグ＆ドロップする
9. `RPI-RP2`が再接続されるのを待つ
10. `GP2040-CE_0.X.X_Haute42.uf2`をドラッグ＆ドロップする
11. `RPI-RP2`の接続が切れるのを待つ

これで最新ファームウェア且つHaute42の設定でアップデートされる。

## Pinマッピング

### 方向

方向ボタンのマッピング

| Pin | GP2040 | 共通 |
| --- | --- | --- |
| 02 | Up | 上 |
| 03 | Down | 下 |
| 04 | Right | 右 |
| 05 | Left | 左 |

### A, B, X, Y

| Pin | GP2040 | XINPUT | Switch | PS3, PS4 |
| --- | --- | --- | --- | --- |
| 06 | B1 | A | B | × |
| 07 | B2 | B | A | ○ |
| 10 | B3 | X | Y | □ |
| 11 | B4 | Y | X | △ |

### RB, LB, RT, LT

| Pin | GP2040 | XINPUT | Switch | PS3, PS4 |
| --- | --- | --- | --- | --- |
| 08 | R2 | RT | ZR | R2 |
| 09 | L2 | LT | ZL | L2 |
| 12 | R1 | RB | R | R1 |
| 13 | L1 | LB | L | L1 |
| 18 | L3 | LS | LS | LS |
| 19 | R3 | RS | RS | RS |

### Other

| Pin | GP2040 | XINPUT | Switch | PS3, PS4 |
| --- | --- | --- | --- | --- |
| 16 | S1 | Back | Minus | SHARE |
| 17 | S2 | Start | Plus | OPTIONS |
| 20 | A1 | Home | Home | PS |
| 21 | A2 | ------ | Capture | Touchpad |

## Hardware

| Pin | GP2040 | Misc |
| --- | --- | --- |
| 14 | Turbo | 05番（左）の上の小ボタン |
| 18 | L3 | 10番（X）の上 |
| 19 | R3 | 07番（B）の下 |
| 26 | L3 | 10番（X）の上 |
| 27 | 上 | 03番（下）の上 |