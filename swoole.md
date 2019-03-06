# swoole 安裝

> 1. sudo pecl install swoole
> 2. /* 在 php.ini 中添加 extension=swoole.so */
> 3. php -i grep "Loaded Configuration File" /* centOS 結果: Loaded Configuration File => /etc/php.ini */
> 4. /* swoole 有載入順序的限制要先載入sockets */
> 5. echo 'extension=sockets.so' >> /etc/php.ini
> 6. echo 'extension=swoole.so' >> /etc/php.ini
> 7.  /* 關掉原先 extension=sockets.so 的設定 centOS 位置 /etc/php.d/20-sockets.ini*/
