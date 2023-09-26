# How-to-set-Clash
> 在linux环境下配置clash代理

---

[Clash for Windows | Github](https://github.com/Fndroid/clash_for_windows_pkg/releases)

![clash for windows](https://img-blog.csdnimg.cn/b13b4d46ce294dc3b43c79098219bc4e.png#pic_center =700x)
- 进入下载目录后解压缩
```shell
tar -zxvf ./Clash.for.Windows-0.20.36-x64-linux.tar.gz
```
- 进入软件目录后双击 `cfw` 打开，或通过终端输入 `./cfw` 打开
- 配置 Clash
![TUN](https://img-blog.csdnimg.cn/3c96d11188ce4ec7a24e89ecfe3c47d1.png#pic_center =500x)
- 配置网络代理
	- 打开有线设置
		![Connection](https://img-blog.csdnimg.cn/0ca0b491b7b14af790dd041d1f2c56bf.png#pic_center =300x)
	- 修改网络代理为手动
	![HTTP](https://img-blog.csdnimg.cn/d3cdec9d12c0479799f5452bd4dd17be.png#pic_center =600x)
- 配置系统代理
	```shell
	vim ~/.bashrc
	```
	- 加入以下行
	```shell
	export https_proxy=http://127.0.0.1:7890
	export http_proxy=http://127.0.0.1:7890
	# export all_proxy=socks5://127.0.0.1:7890
	export no_proxy=localhost,127.0.0.1
	```

