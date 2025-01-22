在本文中，你将学习如何通过 DigitalOcean 的管理面板创建一个 Ubuntu 服务器，并将其配置为使用你的 SSH 密钥。设置好服务器后，你可以在其上部署应用程序和网站。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bit.ly/bewildcard)

## 准备工作

在开始本教程之前，请确保满足以下条件：

- **对命令行有一定的了解**：如果需要复习，可以参考 [Linux 命令行入门](https://www.digitalocean.com/community/tutorials/a-linux-command-line-primer)。
- **SSH 密钥**：用于启用与服务器的安全连接。你可以参考 [如何在 Ubuntu 上设置 SSH 密钥](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04)。
- **信用卡或 PayPal 帐户**：用于设置 DigitalOcean Droplet 云主机。

---

## 步骤 1 — 创建 DigitalOcean 帐户

1. 访问 [DigitalOcean 新帐户注册页面](https://www.digitalocean.com/?refcode=db9b35360821) 创建账户。
2. 输入信用卡或 PayPal 信息以完成账户验证。注意，验证过程中可能会有一笔临时预授权费用，但会在一周内取消。
3. 完成注册后，进入“注册完成”页面，准备开始创建 Droplet。

---

## 步骤 2 — 设置你的 Droplet

1. 点击“让我们做点什么（Let’s make something）”按钮，进入 Droplet 创建页面。
2. 在页面中选择操作系统、内存、存储等配置。

---

## 步骤 3 — 选择操作系统镜像

在操作系统镜像选项中，选择 **Ubuntu (LTS) x64**，然后继续下一步。

---

## 步骤 4 — 选择计划

选择适合你的计划，例如每月 5 美元的基础计划。如果需要更高性能，可以根据需求调整配置。

---

## 步骤 5 — 添加块存储（可选）

如果需要额外的文件存储空间，可以在此步骤添加块存储。否则，直接跳过。

---

## 步骤 6 — 选择数据中心区域

选择离你和你的用户最近的数据中心，以获得最佳性能和最低延迟。

---

## 步骤 7 — 选择其他选项

在此步骤中，你可以启用以下免费功能：

- **IPv6**：启用 IPv6 访问。
- **用户数据**：为 Droplet 提供自定义数据。
- **监控**：收集扩展指标并创建警报策略。

---

## 步骤 8 — 设置 SSH 身份验证

1. 点击“使用 SSH 密钥进行身份验证”选项。
2. 如果尚未创建 SSH 密钥，可以参考 [如何在 Ubuntu 上设置 SSH 密钥](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04)。
3. 将生成的公钥粘贴到云面板中，并为密钥命名。

---

## 步骤 9 — 完成并创建 Droplet

1. 确认 Droplet 的数量、名称和标签。
2. 如果需要，可以启用备份功能（每月额外收费 1 美元）。
3. 点击“创建 Droplet”按钮，等待创建完成。
4. 创建完成后，记录 Droplet 的 IP 地址。

---

## 连接到 Droplet

使用以下命令通过 SSH 连接到你的 Droplet：

bash
ssh root@your_IP_address


首次连接时，系统会提示你确认连接，输入 `yes` 即可。如果一切正常，你将以 root 用户身份登录到 Droplet。

---

## 结论

通过本教程，你已经成功在 DigitalOcean Droplet 上创建了一个 Ubuntu 服务器并启用了 SSH 访问。接下来，你可以根据需要部署应用程序或网站。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bit.ly/bewildcard)