---
title: '[译]Boostrap3 vs 4'
tags:
  - Bootstrap
  - CSS
  - 译
abbrlink: cebcfde4
date: 2018-06-20 06:48:15
---
> Bootstrap于1月19日放出了4的正式版，4带来了一些主要的改变，添加了新的组件，废弃了一些。这里是Bootstrap 3与4的区别

原文链接:[这里](https://www.quackit.com/bootstrap/bootstrap_4/differences_between_bootstrap_3_and_bootstrap_4.cfm)

|组件|Bootstrap 3| Bootstrap 4|
| --- | --- | --- |
|全局|
|CSS源文件|LESS|SCSS|
|CSS主要单位|px|rem|
|媒体查询单位|px|px|
|全局字体大小|14px|16px|
|缺省字体集|Helvetica Neue, Helvetica, Arial, sans-serif|Uses a "native font stack" (user's system fonts), with a fallback to Helvetica Neue, Arial, and sans-serif|
|栅格化|
|栅格参数|4种栅格系统(xs,sm,md,lg)|5种(xs,sm,md,lg,xl) *Bootstrap 4已经删除了最小断点的的xs,因此col-*覆盖了所有所有设备`不再需要标明这种情况得尺寸了`*
|偏移|用col-*-offset-*去偏移列,例如col-md-offset-4|用offset-*-*去偏移列，例如,offset-md-4.|
|表格|
|黑色主题表格|不支持|增加dark表格样式，用`.table-dark`|
|Table表头样式|不支持|`.thead-light` 和 `.thead-dark`|
|紧缩表格|`.table-condensed`|`.table-sm`|
|状态类|Bootstrap 3 不用`.table-`前缀，例如Bootstrap 3 用`.active`然而Bootstrap 4 用`.table-active`,状态关键词都是(active,success,info,warning,danger)|添加`.table-`前缀来做表格的状态类
|响应式表格|`.table-response`类必须添加到父级div元素上|一样，同时增加了`table-responsive-*`来表明断点`.table-responsive{-sm|-md|-lg|-xl}`|
|表单|
|水平表单|
|复选框与单元按钮|
|表单控件尺寸|
|表单Label大小|
|Help Text|用`.help-block`显示帮助信息|`.form-text`|
|校验和反馈图标|包含所有校验状态样式,图标使用的glyphicons|去除校验样式|
|标题|不支持|提供`.col-form-label`用于legend标签|
|固定文本|用`.form-control-static`去渲染固定文本|`.form-control-plaintext`|
|自定义表单|不支持|支持|
|按钮|
|样式|`.btn-secondary`不可用|去掉`.btn-default`，增加了`btn-secondary`,`btn-light`,和`btn-dark`|
|边框按钮|不支持|`btn-outline-*`为按钮增加边框颜色|
|尺寸|`.btn-xs`可用|`.btn-xs`删除,`.btn-sm`,`.btn-lg`可用|
|控件组|
|Classes|使用`.input-group-addon`和`.input-group-btn`|废除了`.input-group-addon`,`input-group-btn`,增加了`input-group-prepend`,`.input-group-append`，也增加了`.input-group-text`用于空间组中文本|
|Glyphicons|
|支持性|支持|不支持|
|非响应式使用|
|支持性|支持|不支持|
|路径导航|
| 轮播 |
|轮播项|用`.item`|用`.carousel-item`
|Affix|
|支持性|支持|不支持|
