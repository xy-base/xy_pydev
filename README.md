<!--
 * @Author: yuyangit yuyangit.0515@qq.com
 * @Date: 2024-10-19 10:23:26
 * @LastEditors: yuyangit yuyangit.0515@qq.com
 * @LastEditTime: 2024-10-19 10:26:56
 * @FilePath: /xy_pydev/README.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# xy_pydev

- [简体中文](readme/README_zh_CN.md)
- [繁体中文](readme/README_zh_TW.md)
- [English](readme/README_en.md)

# 说明
简单Python模块开发工具.

## 源码仓库

- <a href="https://github.com/xy-base/xy_pydev.git" target="_blank">Github地址</a>  
- <a href="https://gitee.com/xy-base/xy_pydev.git" target="_blank">Gitee地址</a>

## 安装

```bash
# bash
pip install xy_pydev
```

## 说明

###### 1. 清理缓存

```bash
# bash
# 删除缓存
xy_pydev -w clean
# ======================================
# 开始清理模块缓存...
# ======================================
# ======================================
# 即将清理包含以下列表中名称的目录或者文件: 
# ['dist', '.egg-info', 'build']
# ======================================
# ======================================
# 检测到以下缓存
# ======================================
# build
# ======================================
# xy_pydev.egg-info
# ======================================
# dist
# ======================================
# ======================================
# 是否确定删除缓存?
# Y ==> [确定]
# 其他 ==> [取消]
# 请输入[Y/n]

```

###### 2. 创建简易模块

```bash
# 当前目录在 /home/helios/workspace/project/opensource/xy-base/xy_pydev/test
xy_pydev
# 出现引导，也可以按需提前设置参数
# ======================================
# 请输入新模块名称, 不能包含中文
# xy_demo
# ======================================
# 新模块名称为: xy_demo
# ======================================
# 是否需要修改模块入口类名称?
# 当前为: Runner
# 不能包含中文
# Y=>代表[需要];
# 其他=>代表[不需要]
# 请输入[ Y/n ]
# ======================================
# 是否需要添加全局命令?
# Y=>代表[添加];
# 其他=>代表[不添加]
# 请输入[ Y/n ]
# ======================================
# 新模块创建完成!!!
```

###### 3. 创建包含全局命令的模块

```bash
xy_pydev
# ======================================
# 请输入新模块名称, 不能包含中文
# xy_full_demo
# ======================================
# 新模块名称为: xy_full_demo
# ======================================
# 是否需要修改模块入口类名称?
# 当前为: Runner
# 不能包含中文
# Y=>代表[需要];
# 其他=>代表[不需要]
# 请输入[ Y/n ]
# ======================================
# 是否需要添加全局命令?
# Y=>代表[添加];
# 其他=>代表[不添加]
# 请输入[ Y/n ]
# Y
# ======================================
# 新模块创建完成!!!
```

###### 4. 指定参数创建模块

```bash
xy_pydev -h
# usage: xy_pydev-1.0.5 [-h] [-w [WORK]] [-n [NAME]] [-m [MODULE_CLASS_NAME]]
#                       [-s [SCRIPTS]]

# python模块开发工具 =====> v1.0.5

# options:
#   -h, --help            show this help message and exit
#   -w [WORK], --work [WORK]
#                         工作方式: 1.clean => 清理模块缓存 2.build => 编译 3.utpi =>
#                         提交到test.pypi.org, upload to test.pypi.org 4.upi =>
#                         提交到pypi.org, upload to pypi.org 5.其他 => 创建项目
#   -n [NAME], --name [NAME]
#                         Python模块名称 不能包含中文
#   -m [MODULE_CLASS_NAME], --module_class_name [MODULE_CLASS_NAME]
#                         模块入口类名称 不能包含中文
#   -s [SCRIPTS], --scripts [SCRIPTS]
#                         是否开启全局命令

xy_pydev -n xy_arg_demo -m ARG_DEMO -s 1
# ======================================
# 新模块名称为: xy_arg_demo
# ======================================
# 新模块创建完成!!!
```

##### <b>提示</b>
在使用 xy_pydev 创建模块后可以引入 
[xy_argparse.github](https://github.com/xy-base/xy_argparse.git)
[xy_argparse.gitee](https://gitee.com/xy-base/xy_argparse.git)
或者
[xy_work.github](https://github.com/xy-base/xy_work.git)
[xy_work.gitee](https://gitee.com/xy-base/xy_work.git)
进行定制和扩展模块的功能.

## 许可证
xy_pydev 根据 <木兰宽松许可证, 第2版> 获得许可。有关详细信息，请参阅 [LICENSE](LICENSE) 文件。

## 捐赠

如果小伙伴们觉得这些工具还不错的话，能否请咱喝一杯咖啡呢?  
![Pay-Total](./readme/Pay-Total.png)


## 联系方式

```
微信: yuyangiit
邮箱: yuyangit.0515@qq.com
```