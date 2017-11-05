## Inside Channels

внутри каналы устроены следующим образом



[http://dmitryvorobev.blogspot.com.es/2016/08/golang-channels-implementation.html](http://dmitryvorobev.blogspot.com.es/2016/08/golang-channels-implementation.html)



![](https://d33ypg4xwx0n86.cloudfront.net/direct?url=https%3A%2F%2Fhabrastorage.org%2Ffiles%2F483%2F025%2F741%2F48302574178048caac81c816f9e37238.png&resize=w640)

qcount - количество элементов в буфереля

dataqsiz -  размерность буфера

buf - указатель на буфер для элементов канала

closed -флаг, указывающий закрыт канал или нет

recvq - указатель на связанный список горутин , ожидающих чтения из канала

sendq - указатель на связанный список горутин, ожидающих запись в канал

lock - мьютекс для безопасного доступа к каналу



