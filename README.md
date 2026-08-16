# zshipu/imagesv5

zshipu 站群图床（第 5 卷），经 jsDelivr 分发：

```
https://cdn.jsdelivr.net/gh/zshipu/imagesv5/<日期>/<文件名>
```

## 收录范围

**2025-10-12 及以后**的图片在本仓库；之前的在 zshipu/imagesv4。
按日期即可判断归属，不需要查表。

## 组织方式

按图片原始日期分目录，例如 `2025-10-04/`。沿用 imagesv3 的分层习惯，
便于按批次定位与清理。

## 由来

站群正文图片原先托管在第三方域名下，可用性不受自己控制——对方一旦停服
或加防盗链，两千多篇文章会同时满屏坏图。因此统一迁入自有图床。

迁移工具在 `webagent/scripts/`：

- `download-site-images.py` —— 限速下载 + 内容校验（拒绝 0 字节、防盗链占位图、HTML 错误页）
- `rewrite-site-images.py` —— 正文图片 URL 改写

## 维护约定

- 仓库必须保持**公开**，否则 jsDelivr 无法分发。
- 单文件不要超过 20 MB（jsDelivr 上限）。
- 体积接近 2 GB 时另起 imagesv6，不要让单个仓库无限膨胀。
- 本地工作副本放在 **E 盘**（`E:\imagesv5`），D 盘空间紧张。
