# rtl8723bs
Realtek SDIO Wi-Fi driver

以下の端末でテストを行いました。
- Onda v975w
- Teclast 3G
- HP Stream 7
- Dell Venue 8 3000
- WinBook TW100 and TW700

そのデバイスが ```/sys/bus/sdio/``` 下にあることを確認してください。

これら全てのタブレットにおいて、BayTrail SDIO ドライバに二、三のパッチを適用する必要があります。

http://thread.gmane.org/gmane.linux.kernel.mmc/25081/focus=25087
http://thread.gmane.org/gmane.linux.kernel.mmc/31583

4.3 より古いカーネルには、このパッチも適用する必要があります。
https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/?id=d31911b9374a76560d2c8ea4aa6ce5781621e81d

これらのパッチは patches/ サブディレクトリの中でも見つけられます。
