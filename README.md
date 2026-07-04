# 情侣存钱小银行（云端记账版）
静态单页网站，可部署 GitHub Pages，搭配 Firebase Realtime Database 实现双人云端同步记账

## 功能
1. 区分微信/支付宝存取渠道
2. 存钱、取钱收支记录，自动计算总余额
3. 支持上传转账截图（Base64存入云端）
4. 单条记录编辑、删除
5. 多设备实时同步数据

## 使用部署教程
### 1. 本地使用
直接双击 index.html 打开即可（无 Firebase 配置无法云端存储）

### 2. GitHub Pages 线上部署
1. 新建公开仓库，上传 index.html 和 README.md
2. 仓库 Settings → Pages
3. Source 选择 Deploy from a branch，分支 main，文件夹根目录 /
4. 等待2-5分钟，访问地址：`你的用户名.github.io/仓库名`

### 3. Firebase 配置步骤
1. 前往 Firebase 官网创建项目，开启 Realtime Database
2. 获取项目配置密钥，替换 index.html 内 `firebaseConfig` 对象
3. 修改数据库规则允许读写，即可云端同步

## 项目结构