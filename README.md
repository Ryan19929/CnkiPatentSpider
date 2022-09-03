# CnkiPatentSpider

知网专利爬虫（前1-2步），得到的数据是专利公开号列表。

需要和另外一个项目配合，仅供学习交流使用。

## 功能
分两步，为了保证尽可能地存储过程中的 html 信息，防止后面返工

### 第一步
* 输入
  * 开始日期和结束日期
  * 学科分类号列表
* 输出
  * 所有专利搜索结果的 html 源文件，以形如 `2021-01-01/A001_1/1.html` 的文件名命名，其中 `1.html` 代表第一页

### 第二步

* 输入
  * 前一步得到的所有专利搜索结果的 html 源文件
* 输出
  * 三元组
    * 日期
    * 学科分类号
    * 专利公开号
  * 目前是存到数据库里