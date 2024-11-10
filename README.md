# Nodepay.ai
![Nodepay.ai](image.png)
Nodepay.ai 机器人使用多个代理自动 ping

注册 Nodepay.ai : [https://app.nodepay.ai/register](https://app.nodepay.ai/register?ref=alOvt9MJJxpdRTK)

# 功能
此脚本旨在在服务器上使用多个代理运行。

# 运行代码的步骤
```bash
git clone https://github.com/Gzgod/nodepaynew.git
cd nodepaynew
```
**更新代理**
```bash
wget https://raw.githubusercontent.com/monosans/proxy-list/main/proxies/all.txt && mv all.txt proxy.txt
每个账户最多可以连接10个代理
所以现在最好的耕种方式是手动创建多个账户
该脚本支持多账户，只需np_tokens.txt为 1 个账户每行粘贴令牌即可
确保你的帐户获得人类证明徽章
```
## 1. 获取所需信息

1. 打开链接并登录 [https://app.nodepay.ai/](https://app.nodepay.ai/register?ref=Od15EPpf6UBd5qR)
2. 按 F12 打开控制台，并输入代码（Ctrl + Shift + i 进行检查）
3. 在控制台中输入 ``localStorage.getItem('np_token');``
4. 控制台中打印的文本就是您的 NP_TOKEN，复制并粘贴到 `np_token.txt`
5. 将您的代理放入 `proxy.txt` 文件中，例如：`http://username:pass@ip:port`
## 2. 安装依赖
```bash
pip install -r requirements.txt
```
## 3. 运行脚本
```bash
python3 main.py
```
## 预期输出
如果运行正常，您将看到如下日志：
```bash
2024-07-30 04:37:18.263 | Ping 成功: {'success': True, 'code': 0, 'msg': '成功', 'data': {'ip_score': 88}}
2024-07-30 04:37:48.621 | Ping 成功: {'success': True, 'code': 0, 'msg': '成功', 'data': {'ip_score': 90}}
2024-07-30 04:38:18.968 | Ping 成功: {'success': True, 'code': 0, 'msg': '成功', 'data': {'ip_score': 94}}
2024-07-30 04:38:59.338 | Ping 成功: {'success': True, 'code': 0, 'msg': '成功', 'data': {'ip_score': 98}}
```

--- 
