<!--
 * @Author: yuyangit yuyangit.0515@qq.com
 * @Date: 2024-10-19 10:23:23
 * @LastEditors: yuyangit yuyangit.0515@qq.com
 * @LastEditTime: 2024-10-19 10:38:37
 * @FilePath: /xy_pydev/readme/README_en.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->

# xy_pydev

- [简体中文](README_zh_CN.md)
- [繁体中文](README_zh_TW.md)
- [English](README_en.md)

# Description
Simple Python module development tool.

## Source Code Repositories

- <a href="https://github.com/xy-base/xy_list.git" target="_blank">Github</a>  
- <a href="https://gitee.com/xy-base/xy_list.git" target="_blank">Gitee</a>

## Installation

```bash
# bash
pip install xy_pydev
```

## Illustrate

###### 1. Clear cache

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

###### 2. Create a simple module

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

###### 3. Create a module containing global commands

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

###### 4. Specify parameters to create a module

```bash
xy_pydev -h
# usage: xy_dev [-h] [-w [WORK]] [-n [NAME]] [-m [MODULE_CLASS_NAME]]
#               [-s [SCRIPTS]]
# python模块开发工具
# options:
#   -h, --help            show this help message and exit
#   -w [WORK], --work [WORK]
#                         工作方式: 1.clean => 清理模块缓存 2.其他 => 创建项目
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


## License
xy_pydev is licensed under the <Mulan Permissive Software License，Version 2>. See the [LICENSE](../LICENSE) file for more info.

## Donate

If you think these tools are pretty good, Can you please have a cup of coffee?  

![Pay-Total](./Pay-Total.png)  


## Contact

```
WeChat: yuyangiit
Mail: yuyangit.0515@qq.com
```