iCMS模板标签
====
##站点信息
```html
<!--{$site}-->
```
###使用范围
- 所有模板

###数据结构
```html
Array(
    [name]        => 网站名称
    [seotitle]    => 网站标题
    [keywords]    => 关键字
    [description] => 网站描述
    [icp]         => 备案号
    [title]       => 网站名称 (name的别名)
    [404]         => 404页面 网址
    [url]         => 网站网址
    [tpl]         => 当前模板目录
    [urls]        => Array(
        [tpl]    => 当前模板目录URL
        [public] => 公共资源URL
        [user]   => 用户URL
        [res]    => 附件URL
        [ui]     => 系统UI URL
        [avatar] => 用户头像URL
    )
)
```
###调用方式

```html
网站名称:<!--{$site.name}-->
公共资源URL:<!--{$site.urls.public}-->
```
