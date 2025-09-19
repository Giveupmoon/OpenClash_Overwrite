# OpenClash_Overwrite
OpenClash覆写模块相关文件

建议新装OpenClash使用，不需要修改任何luci设置

需要OpenClash	v0.47.006及以上版本使用

建议切换更新分支为Dev 并启用Smart

本仓库覆写模块默认开启Smart智能策略组 开启数据收集并定义数据收集文件最大大小为500Mb 且关闭使用LightGBM模型

建议使用一段时间后自行训练模型替换使用

分流规则及策略组基于项目：[Aethersailor/Custom_OpenClash_Rules](https://github.com/Aethersailor/Custom_OpenClash_Rules.git)

使用方法：

新增覆写模块：

订阅链接

文件名可自定义

类型：http

订阅链接为：
```
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite.conf
```
注意定义环境变量：
```
EN_KEY=你的机场订阅链接
```
保存 去其他配置页底部点一手应用配置即可


温馨提示：
本仓库文件内引用的各种链接均为原始链接，使用时注意需路由本身可访问GitHub

满足上述前提下，前几次运行启动成功后会提示内核错误，重启几次即可

（默认OpenClash没GeoIP数据库）第一次运行就是它下载去了，不能热重载导致第一次会运行错误

当然你也可以手动提前更新一下GeoIp dat
