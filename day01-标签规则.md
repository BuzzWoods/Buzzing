# 标签

## 标签的嵌套的规则

- 块级标签嵌套块级标签（注意：不能标题标签嵌套段落标签内）
```

错误示例：

    <p style="color:blue;">
        <h1>1234</h1>  不会继承p的颜色！
    </p>

```
- ul，li（无序列表）、ol，li（有序列表）、dl，dt，dd（自定义列表）为固定搭配，li只能嵌入ul内，li可嵌套div
- 内联可嵌套内联，但不能嵌套块级

## 相对路径

- \后面为下级目录
- .\为当前目录
- ..\为返回上一级目录

## 空标签

- href="#" 跳回顶部
- href="" 跳回顶部
- href="javascript:void(0);" 不跳回顶部，推荐使用

## 锚点链接（跳转到需要位置）：

- 同页面下：href="#目标id值"
- 其它页面下：href="文件相对路径#目标id值"

## 表格：

- <thead>/<tbody>/<thead>用于区分表格部分，在html中调换顺序不会影响页面布局
- rowspan跨行合并（纵向）、colspan跨列合并（横向）

## 表单：

- 表单的密码显示：type为password才能有隐私显示
- form内action为数据传输的路径，method内post和get为传输方式，get从服务器内获取数据，post将当前数据传入服务器
- type="checkedbox" checked中checked为默认选择选项
- type为radios时，选项设置name为同一值，才能实现单选
- 文本域textarea 高宽可用rows和cols设置，设置的值是字符长度；内部的三角用css消除-resize：none；
- maxlength输入的最大值，字符长度；readonly-只读，disable-禁用
- optgroup 选择内部分类标签