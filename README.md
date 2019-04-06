# ChbImageLoader
自己写的ImageLoader。具备：

- 图片同步加载
- 图片异步加载
- 图片压缩
- 内存缓存
- 磁盘缓存
- 网络拉取



#### 三级缓存

​	通过LruCache、DiskLruCache实现内存缓存和磁盘缓存。需要使用一张图片时，先在LruCache内查找是否有缓存，没有则查找DiskLruCache，两者都没有，则进行网络拉取。



#### 图片压缩

​	用于显示图片的imageview有时比图片小，所以缓存的时候，可以对图片进行压缩，只缓存需要使用的大小，避免浪费内存，提高性能。



#### 效果图

![https://github.com/XINANbang/ChbImageLoader/blob/master/image/previewe.jpg]()	

