# 2020Robosys

このプログラムは上田隆一先生が担当する2021年ロボットシステム学の課題で作成したものであり,  Rasberry Pi4に接続したLEDを点灯させるプログラムである.
講義動画内で上田先生が作成したプログラムを参考にしている. 

●動作環境
・Rasberry Pi 4 
・Os : Ubuntu 20.04 server

●使用したもの
・Rasberry Pi 4
・LED(赤) x 1
・抵抗 220Ω x 1
・ブレッドボード BB-601(白) x 1
・ジャンパー線 x 1

●使用方法

【インストール】
$ git clone https://github.com:yuikadomura/2021-12-10.git
$ cd 2021-12-10
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0

【アンインストール】
$ sudo rmmod myled
$ make clean

【LED(赤)を点灯する】
$ echo 1 > /dev/myled0

【LED(赤)を消灯する】
$ echo 0 > /dev/myled0

●実行時の動画
https://t.co/x2qWj111Z6
