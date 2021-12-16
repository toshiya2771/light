# light

講義第7・8回で作成したmyled.cを使って、LEDを光らせます

# Demo
youtubeに動画を上げました
https://www.youtube.com/watch?v=ka_I6uXFfIQ

# Use
Raspberry Pi 4 Model B
ブレッドボード
ジャンパー線
抵抗（Φ5）
LED(青色)

# Usage
make /n
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
echo 1 > /dev/myled0 (ledを光らせる)
echo 0 > /dev/myled0 (ledを消す)
sudo rmmod myled



