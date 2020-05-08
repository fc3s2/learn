[来源](https://man.linuxde.net/ "linux")

### tar
#### 

* 
* 
#### 选项 

| 字段名 |  说明 |
| :------|  :------ |
| -A or --catenate | 新增文件到以存在的备份文件 |
| -B  | 设置区块大小 |
| -c or --create  | 建立新的备份文件 |
| -C <目录>  | 这个选项用在解压缩,若要在特别目录解压缩,可以使用这个选项 |
| -d | 记录文件的差别 |
| -x or --extract or --get  | 从备份文件中还原文件 |
| -t or --list  | 列出备份文件的内容 |
| -z or --gzip or --ungzip  | 通过gzip指令处理备份文件 |
| -f  | 指定备份文件 |
| -v or --verbose | 显示指令执行过程 |
| -r  | 添加文件到已经压缩的文件 |
| -u  | 添加改变了和现有的文件到已经存在的压缩文件 |
| -j  | 支持bzip2解压文件 |
| -v  | 显示操作过程 |
| -l  | 文件系统边界设置 |
| -k  | 保留原有文件不覆盖 |
| -m  | 保留文件不被覆盖 |
| -w  | 确认压缩文件的正确性 |
| -p --same-permissions | 用原来的文件权限还原文件 |
|-P --absolute-names|文件名使用绝对名称，不移除文件名称前的“/”号 |
|-N <日期格式> or--newer=<日期时间>|只将较指定日期更新的文件保存到备份文件里|
|--exclude =<范本样式>|排除符合范本样式的文件|

买了服务器,运行了一段时间服务器硬盘容量不够了

阿里云扩容
https://help.aliyun.com/document_detail/111738.html?spm=a2c4g.11186623.4.1.6b814c07wjlpdY

growpart <DeviceName> <PartionNumber>