Shopee 多站点利润模拟器 V6.2（方案二：网页与数据分离）

目录结构：
index.html
data/sku-cost.json
data/warehouse-fee.json

部署：
1. 将整个文件夹内容上传到 GitHub 仓库根目录。
2. 保持 data 文件夹和 index.html 的相对位置不变。
3. Vercel 会自动重新部署，原网址不变。

后续更新成本：
- 只替换 data/sku-cost.json。
- 印尼仓储费用变化时，只替换 data/warehouse-fee.json。
- 提交 GitHub 后，Vercel 自动更新。

重要：
- 因为网页通过 fetch 读取 JSON，不能直接双击 index.html 测试。
- 应通过 Vercel 网址访问，或在本机使用 HTTP 服务器。
- JSON 文件属于公开静态资源，任何能访问网址的人理论上都能读取其中数据。
