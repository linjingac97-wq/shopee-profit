# Shopee利润核算工具

本项目基于之前确认可用的 V6.1 页面拆分，只把内置数据独立为 JSON 文件，未改动原有印尼、越南核算逻辑。

## 正确目录

```text
index.html
vercel.json
data/
  sku-cost.json
  warehouse-fee.json
```

## 上传 GitHub

1. 先解压部署包，不要把 ZIP 本身上传。
2. 打开原 GitHub 仓库。
3. 删除旧的 index.html、旧 data 文件夹和错误的 index.html.html。
4. 把本包中的 index.html、vercel.json、data 文件夹上传到仓库根目录。
5. 点击 Commit changes。
6. 等待 Vercel 自动部署显示 Ready。
7. 用 Ctrl + F5 强制刷新原网址。

## 后续数据更新

- SKU、成本、产品状态、SKU数量、组合关系更新：只替换 data/sku-cost.json。
- 印尼仓储费用更新：只替换 data/warehouse-fee.json。
- 公式或页面功能变化：才更新 index.html。

注意：必须通过 Vercel 网址访问。直接双击 index.html 时，浏览器可能阻止读取 JSON 文件。
