# 阿里云日志服务(SLS)插件
**作者:** lework
**版本:** 0.0.1
**类型:** tool
**REPO:** [dify-plugins-aliyun-sls](https://github.com/lework/dify-plugins-aliyun-sls)

这是一个用于查询阿里云日志服务(SLS)中日志数据的 Dify 插件。

## 功能

- 查询阿里云 SLS 日志服务中的日志数据
- 支持指定查询语句、日志库、时间范围等参数
- 支持自定义查询结果数量限制

## 配置

使用此插件需要提供以下阿里云凭证信息：

- Endpoint: 阿里云 SLS 服务的 Endpoint，例如：cn-hangzhou.log.aliyuncs.com
- Access Key ID: 阿里云账号的 Access Key ID
- Access Key Secret: 阿里云账号的 Access Key Secret
- Project: 阿里云 SLS 的项目名称
- Logstore (可选): 阿里云 SLS 的日志库名称，也可在查询时指定

## 使用示例

```
查询最近15分钟内包含"error"的日志
```

```
查询logstore为"nginx-access"中最近1小时的所有日志，限制返回50条
```

## 查询语法

支持阿里云 SLS 的查询语法，详情请参考[阿里云 SLS 查询语法文档](https://help.aliyun.com/document_detail/29060.html)。
