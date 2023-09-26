# How-to-set-Clash
> 在linux环境下配置clash代理

---

[Clash for Windows | Github](https://github.com/Fndroid/clash_for_windows_pkg/releases)

![clash for windows](https://github.com/MorphBai/How-to-set-Clash/blob/main/clash%20for%20windows.png)
- 进入下载目录后解压缩
```shell
tar -zxvf ./Clash.for.Windows-0.20.36-x64-linux.tar.gz
```

- 进入软件目录后双击 `cfw` 打开，或通过终端输入 `./cfw` 打开

- 配置 Clash

![set clash](https://github.com/MorphBai/How-to-set-Clash/blob/main/set%20clash.png)

- 配置网络代理
	- 打开有线设置

	![network proxy](https://github.com/MorphBai/How-to-set-Clash/blob/main/network%20proxy.png)

	- 修改网络代理为手动

	![set network proxy](https://github.com/MorphBai/How-to-set-Clash/blob/main/set%20network%20proxy.png)

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

