# Google Search Console 设置指南

## 1. 验证网站所有权

### 方法A：HTML文件验证（推荐）

1. 访问 [Google Search Console](https://search.google.com/search-console)
2. 点击 "添加资源" → "网址前缀"
3. 输入：`https://www.setrendtech.com`
4. 选择验证方法："HTML文件"
5. 下载验证文件（如：googlea77be25917777b72.html）
6. 上传到网站根目录
7. 点击验证

**注意：** 项目中的 `googlea77be25917777b72.html` 是示例文件，请使用Google生成的实际文件。

### 方法B：HTML标记验证

在 `<head>` 中添加：
```html
<meta name="google-site-verification" content="你的验证码" />
```

### 方法C：DNS验证

在域名DNS设置中添加TXT记录：
```
名称：@
类型：TXT
值：google-site-verification=你的验证码
```

---

## 2. 提交网站地图

验证成功后：

1. 在Search Console左侧菜单点击 "网站地图"
2. 在 "添加新的网站地图" 中输入：
   ```
   sitemap.xml
   ```
3. 点击 "提交"

---

## 3. 请求索引新页面

对于 spot-goods.html：

1. 在Search Console顶部搜索框输入：
   ```
   https://www.setrendtech.com/spot-goods.html
   ```
2. 点击 "请求编入索引"
3. 等待Google抓取（通常1-7天）

---

## 4. 检查索引状态

在Google搜索：
```
site:setrendtech.com
```

查看已收录的页面数量。

---

## 5. 优化建议

### 定期更新
- 每周更新现货数据
- 每月检查索引状态
- 每季度审查搜索表现

### 监控指标
- 总点击次数
- 总展示次数
- 平均点击率
- 平均排名位置

### 常见问题
**Q: 页面已上传但搜不到？**
A: 需要等待Google抓取，通常1-7天。可通过Search Console手动请求索引。

**Q: 描述显示旧内容？**
A: Google缓存需要时间更新，可通过Search Console请求重新抓取。

**Q: 如何加速收录？**
A: 
1. 确保网站可访问
2. 提交sitemap
3. 手动请求索引
4. 获取外部链接

---

## 6. 文件清单

上传以下文件到服务器根目录：

```
setrendtech-new/
├── index.html
├── led.html
├── power.html
├── applications.html
├── about.html
├── contact.html
├── spot-goods.html      ← 新增
├── sitemap.xml          ← 已更新
├── robots.txt
├── google-site-verification.html  ← Google生成的验证文件
└── images/
```

---

## 7. 验证步骤

1. ✅ 确认所有文件已上传
2. ✅ 访问 https://www.setrendtech.com/spot-goods.html 正常显示
3. ✅ 在Search Console验证网站
4. ✅ 提交 sitemap.xml
5. ✅ 请求索引 spot-goods.html
6. ⏳ 等待1-7天
7. ✅ 搜索 `site:setrendtech.com LXZ1-PR01` 检查

---

**设置完成时间：** 2026-05-15
**预计生效时间：** 1-7个工作日
