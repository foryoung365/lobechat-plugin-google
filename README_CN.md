# LobeChat Google Custom Search 插件

使用 [Google Custom Search API](https://developers.google.com/custom-search) 的LobeChat搜索插件。

## 设置步骤

1. 创建 Google Custom Search Engine
   - 访问 [Google Programmable Search Engine](https://programmablesearch.google.com/create)
   - 创建一个自定义搜索引擎
   - 获取您的搜索引擎ID (cx参数)

2. 获取 Google API 密钥
   - 访问 [Google Cloud Console](https://console.cloud.google.com/)
   - 创建一个项目
   - 启用 "Custom Search API"
   - 创建API密钥 (key参数)

3. 在LobeChat中配置插件
   - 将此插件添加到LobeChat
   - 在配置页面中提供您的API密钥和搜索引擎ID
   - 这些凭据会作为安全参数自动添加到每个请求中

## 认证方式

此插件使用以下两个安全参数:
- `key`: 您的Google API密钥
- `cx`: 您的自定义搜索引擎ID

这两个参数会作为查询参数添加到API请求中。

## 限制

- Google Custom Search API 免费版每天限制100次查询
- 付费版可获得更多配额

## 隐私

- 您的搜索查询将发送到Google
- 此插件不会收集或存储您的个人数据

`(与上述任何实体无关联)`
