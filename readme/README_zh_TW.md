<!--
 * @Author: yuyangit yuyangit.0515@qq.com
 * @Date: 2024-10-19 10:23:23
 * @LastEditors: yuyangit yuyangit.0515@qq.com
 * @LastEditTime: 2024-10-19 10:28:26
 * @FilePath: /xy_pydev/readme/README_zh_TW.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# xy_pydev

- [简体中文](README_zh_CN.md)
- [繁体中文](README_zh_TW.md)
- [English](README_en.md)

# 说明
簡單Python模組開發工具.

## 程式碼庫

- <a href="https://github.com/xy-base/xy_pydev.git" target="_blank">Github位址</a>  
- <a href="https://gitee.com/xy-base/xy_pydev.git" target="_blank">Gitee位址</a>

## 安装
```bash
# bash
pip install xy_pydev
```

## 說明

###### 1. 清理快取

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

###### 2. 建立簡易模組

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

###### 3. 建立包含全域命令的模組

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

###### 4. 指定參數建立模組

```bash
xy_pydev -h
# usage: xy_pydev-1.0.8 [-h] [-w [WORK]] [-n [NAME]] [-m [MODULE_CLASS_NAME]] [-s [SCRIPTS]]

# python模块开发工具

# options:
#   -h, --help            show this help message and exit
#   -w [WORK], --work [WORK]
#                         工作方式: 1.clean | c => 清理模块缓存, 2.build | b => 编译, 3.utpi | ut => 提交到test.pypi.org, upload to test.pypi.org, 4.upi | u => 提交到pypi.org, upload to pypi.org, 5.其他 => 创建项目
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
在使用 xy_pydev 建立模組後可以引入
[xy_argparse.github](https://github.com/xy-base/xy_argparse.git)
[xy_argparse.gitee](https://gitee.com/xy-base/xy_argparse.git)
或者
[xy_work.github](https://github.com/xy-base/xy_work.git)
[xy_work.gitee](https://gitee.com/xy-base/xy_work.git)
進行自訂和擴充模組的功能.

## 許可證
xy_pydev 根據 <木蘭寬鬆許可證, 第2版> 獲得許可。有關詳細信息，請參閱 [LICENSE](../LICENSE) 文件。

## 捐贈

如果小夥伴們覺得這些工具還不錯的話，能否請咱喝一杯咖啡呢?  

![Pay-Total](./Pay-Total.png)

## 聯繫方式

```
微信: yuyangiit
郵箱: yuyangit.0515@qq.com
```