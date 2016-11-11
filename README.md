# PCBA TEST

## Usage

### 编译并拷贝到开发板中

	git clone git@github.com:54shady/pcba_test.git android_top_root/external/
	mmm external/pcba_test
	adb push pcba_core /system/bin/

### 使用

- 把res目录里的配置文件拷贝到开发板里的/res/目录下

```shell
	# cd external/pcba_test/
	# for f in `ls`; do adb push $f /res/; done
```

- 关闭android显示刷新,并运行测试

```shell
	# stop
	# pcba_core
```

- 测试完后重新开启android显示

```shell
	# start
```
