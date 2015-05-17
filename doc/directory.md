iCMS模板系统
====

### 模板文件及目录结构
```tree
/template [模板目录]
 ├─default ------------------[默认模板]
 │   article.htm ------------[内容页]
 │   article.up_down.htm ----[内容顶踩功能]
 │   category.index.htm -----[栏目首页]
 │   category.list.htm ------[栏目列表页]
 │   footer.htm -------------[页脚]
 │   header.htm -------------[页头]
 │   index.htm --------------[首页]
 │   public.ui.htm ----------[UI资源]
 │   search.htm -------------[搜索结果页]
 │   tag.index.htm ----------[标签页]
 ├─iCMS ---------------------[系统模板]
 │ │ agreement.htm ----------[服务协议]
 │ │ public.common.htm ------[系统通用页]
 │ │ public.dialog.htm ------[系统对话框]
 │ │ public.ui.htm  ---------[系统UI]
 │ │ sitemap.baidu.htm ------[百度站长平台sitemap模板]
 │ │ sitemap.index.htm ------[百度站长平台sitemap index模板]
 │ │ weixin.api.htm ---------[微信公众平台接口]
 │ ├─comment ----------------[系统评论模板目录]
 │ │   api.json.htm ---------[评论JSON]
 │ │   form.default.htm -----[评论框]
 │ │   form.iframe.htm ------[评论框-框架调用]
 │ │   list.default.htm -----[评论列表模板]
 │ │   list.iframe.htm ------[评论列表模板-框架调用]
 │ └─user  ------------------[用户模板目录]
 │   │ card.htm -------------[用户名片对话框]
 │   │ footer.htm -----------[用户通用页脚]
 │   │ home.article.htm -----[用户主页文章列表]
 │   │ home.favorite.htm ----[用户主页文章列表]
 │   │ home.htm -------------[用户主页]
 │   │ login.close.htm ------[关闭登陆]
 │   │ login.htm ------------[登陆页]
 │   │ manage.htm -----------[用户内容管理页]
 │   │ menu.htm -------------[下拉菜单]
 │   │ profile.htm ----------[用户资料管理页]
 │   │ register.close.htm ---[注册关闭页]
 │   │ register.htm ---------[注册页]
 │   ├─manage ---------------[用户内容管理目录]
 │   │   article.htm --------[用户文章管理]
 │   │   category.htm -------[用户栏目管理]
 │   │   comment.htm  -------[用户评论管理]
 │   │   fans.htm  ----------[用户粉丝管理]
 │   │   favorite.htm  ------[用户收藏管理]
 │   │   follow.htm ---------[用户关注管理]
 │   │   inbox.htm  ---------[用户信息管理]
 │   │   publish.htm  -------[用户文章发布]
 │   └─profile --------------[用户资料管理目录]
 │       avatar.htm ---------[用户头像上传]
 │       base.htm -----------[用户基本信息]
 │       bind.htm -----------[用户绑定开放平台]
 │       custom.htm ---------[用户主页封面]
 │       setpassword.htm ----[用户密码修改]
 ├─mobile -------------------[手机版模板 同默认模板]
 │ │ article.htm
 │ │ category.index.htm
 │ │ category.list.htm
 │ │ footer.htm
 │ │ index.htm
 │ │ navbar.htm
 │ │ public.common.htm
 │ │ public.ui.htm
 │ │ search.htm
 │ │ tag.index.htm
 │ └─user -------------------[手机版用户模板 同iCSM下的user模板]
 │   │ home.htm
 │   │ login.close.htm
 │   │ login.htm
 │   │ manage.htm
 │   │ menu.htm
 │   │ navbar.htm
 │   │ profile.htm
 │   │ register.close.htm
 │   │ register.htm
 │   ├─manage
 │   │   article.htm
 │   │   category.htm
 │   │   comment.htm
 │   │   inbox.htm
 │   │   publish.htm
 │   └─profile
 │       avatar.htm
 │       base.htm
 │       bind.htm
 │       custom.htm
 │       setpassword.htm
 └─weixin -------------------[微信端模板 同默认模板]
    article.htm
    category.index.htm
    category.list.htm
    footer.htm
    index.htm
    navbar.htm
    tag.index.htm
```
> 以上是系统默认的模板命名，除了 iCMS [系统模板] 和 user [用户模板] 外其它模板可以随意命名

**iCMS [系统模板] 和 user [用户模板]**

- 在没有指定的默认底层模板的时候，系统将自动调用这个文件夹的相应文件作为底层模板
- 如果无相关系统模板 默认优化级 为 设备模板-> 手机模板-> 桌面模板

