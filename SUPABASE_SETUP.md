# Supabase Setup

## 你需要先在 Supabase 网页完成

1. 打开 https://supabase.com/ 并登录。
2. 点击 New project。
3. Organization 选择默认即可。
4. Project name 建议填写 `italiano-checkin`。
5. Region 选择离你和学生较近的区域。
6. Database password 自己保存好，不要发给我。
7. 创建完成后，进入 Project Settings -> API。
8. 复制并发给我这两个值：
   - Project URL
   - anon public key

当前已从 anon key 解析到你的 Project URL：

```text
https://imzxxbxdjwqfduwsqipz.supabase.co
```

## 不要发给我

- service_role key
- 数据库密码
- 你的 Supabase 登录密码

## 我拿到 URL 和 anon key 后会做

1. 在 Supabase 建表。
2. 导入当前 `data.json` 的用户、聊天、打卡、作业数据。
3. 把 `index.html` 的数据层从 GitHub `data.json` 切换到 Supabase。
4. 保留 GitHub Pages 作为静态网站。
5. 验证新用户注册、登录、删除用户、打卡、聊天刷新、长按隐藏消息。
6. 提交新版代码到 GitHub Pages。

## 目标

GitHub 只负责托管网页，不再充当数据库。注册、登录、聊天和打卡数据全部进入 Supabase，从根源上消除 GitHub API 写入失败、sha 冲突、PWA 旧缓存和本地/远端数据不一致造成的问题。
