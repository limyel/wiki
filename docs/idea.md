# Idea

强大的 IDE。

## 设置

### 调整窗口字体大小

勾选上 *Preferences | Settings | Editor | General* 下的 *Change font size with Command + Mouse Wheel* 选项之后，我们就可以直接使用 `⌘+鼠标滚轮`（Mac）/ `Ctrl+鼠标滚轮`(Windows&Linux)来更改窗口字体的大小。

### 配置类注释模板

修改 *Preferences | Settings | Editor | File adn Code Templates* 下的 `Class` 和 `Enum` 的模板。例如：

```
/**
 * @author limyel
 * @date ${YEAR}/${MONTH}/${DAY} ${HOUR}:${MINUTE}
 **/
public class ${NAME} {
}

```

### 优化 Live Templates

即编码模板，例如当输入 `sout` 时会直接编程输出语句。该功能在  *Preferences | Settings | Editor | Live Templates* 下配置。

### 全局设置 SDK

修改 *File | New Projects Setup | Structure...| Project* 下的 Project SDK 选项，将其更改为最常用的 Java 版本。这样一来，导入或者新建项目时就会使用改版本的 JDK。

### 自动导包、删除没用的包

勾选上 *Preferences | Settings | Editor | General | Auto Import* 下的指定选项即可。

* Add unambiguous imports on the fly：当没有多个同名包时，自动导入。
* Optimize imports on the fly：自动删除没用到的包。

### 显示方法分割线

勾选上 *Preferences | Settings | Editor | General | Appearance* 下的 Show method separators 选项。

### 显示某个文件的提交记录

在界面左侧空白区域邮件，勾选上 *Annotate with Git Blame* 即可。



## 插件

### Rainbow Brackets

用不同的颜色来指示不同层次的括号。



## 快捷键

### 查看当前类的结构层次

`Ctrl+H`

当我们想要知道一个类有哪些父类或者抽象类、接口有哪些实现类的时候，可以在类名、接口名上使用该快捷键就会在右边栏展示出这些信息。

### 查看类结构

`Alt+7`、`⌘+7`

在类的任意位置使用该快捷键，左边栏就会出现该类所有的属性、方法。

### 检索类

`Ctrl+N`、`⌘+O`

快速检索类或文件

### 关键字检索

`Ctrl+f`、`Ctrl+Shift+f`、`⌘+f`、`⌘+Shift+f `

当前文件/全局检索。

### 查看方法、类的实现

`Ctrl+Alt+B`、`⌘+Alt+B`

在某个方法名或者类名上使用该快捷键，就会跳转到该方法或类的实现，如果只有多个实现，会跳出一个列表供用户选择。

### 查看方法、类在哪些地方被使用

`Alt+Shift+F7`

在方法名或类名上使用该快捷键，下边栏会展示出其在哪些地方被使用了。

### 查看最近使用的文件

`Ctrl+E`、`⌘+E`

使用该快捷键会跳出最近使用过的文件。

### 查看图表形式的类继承

右键类名，选择 *Diagrams | Shw Diagrams* 即可查看图表形式的类继承链。