# 功能介绍

购买有正版授权的用户可直接打开 Office 应用程序并登录微软账号即可激活 Office.

如果之前安装过 Office，可能会因为之前的激活信息残留而导致奇奇怪怪的问题。遇到此类问题可以在许可证管理或者密钥管理里面找到“清除激活信息”。

## 许可证说明

### 零售（Retail）许可证

零售许可证只能使用密钥激活，对于 Microsoft 365（Office 365）系列产品，只能通过登录拥有正版许可证微软账户激活。

目前大多数的零售许可都与微软账户绑定，因此零售版产品激活通常不需要借助 Office Tool Plus 即可完成。

### 批量（Volume）许可证

批量许可证可以使用密钥激活，也能使用 KMS 激活。

- MAK 指的是批量激活密钥（Multiple Activation Key），该密钥有激活次数上限，可以多次使用并激活 Office.
- KMS 激活指的是使用密钥管理服务（Key Management Service）进行激活，KMS 激活需要使用 GVLK，并设置 KMS 主机。

在激活信息不丢失的情况下，使用 MAK 激活为永久激活。

KMS 续期策略由 KMS 主机决定。通常情况下，一次激活的有效期是 180 天，每隔 7 天续期一次。

## 许可证管理

如果系统上没有安装 Office，或者安装的 Office 的版本过于陈旧，则 Office Tool Plus 不会读取 Office 的许可证信息，也就不会在下拉列表中显示许可证。

### 安装许可证

你可以从下拉列表中找到你需要的许可证，然后点击安装许可证以开始操作。Office Tool Plus 为零售版证书内置了默认密钥，为批量版证书内置了 GVLK 密钥。所以你在安装了批量版证书后，不需要额外安装 GVLK 密钥即可直接使用 KMS 激活。

安装证书时，原有的证书不会被覆盖也不会被清除，因此证书会共存。

### 安装其他许可证

如果你需要，你可以安装其他许可证，通常情况下，Office 许可证储存在 `C:\Program Files\Microsoft Office\root\Licenses16`，你可以复制给其他计算机使用。该功能不会安装密钥，需要自行安装密钥。

### 重置许可证状态

此功能会将许可证重置为未激活状态，可以选择重置所有许可证，也可以选择重置特定许可证。

### 清除所有许可证

此功能会删除系统上安装了的所有的 Office 许可证，不会清除密钥。

## 密钥管理

### 安装密钥

输入一个完整的 Office 密钥即可进行密钥的安装。如果你在安装密钥的时候提示“未找到产品 SKU”，请确保你已经安装该密钥对应的许可证。

密钥示例如下：XXXXX-XXXXX-XXXXX-XXXXX-XXXXX

### 卸载密钥

输入密钥的最后五位即可进行密钥的卸载，你可以通过“查看激活信息”找到密钥信息。

### 查看安装 ID (IID)

此功能会显示每个许可证的安装 ID，此 ID 用于电话激活时提供。

### 安装确认 ID (CID)

此功能允许你输入一个确认 ID，用于电话激活。

## KMS 管理

KMS 主机可以是一个域名，也可以是一个 IP 地址，例如：kms.example.com 或者 192.168.123.1

KMS 主机的默认端口是 1688，如果需要，可以手动输入指定为其他端口。

你可以单独应用端口，也可以和主机地址一同设置。当 KMS 端口不为空时，点击保存设置将会同时保存端口设置。

## 清除激活状态

此功能会删除系统上所有的 Office 许可证、密钥，你的 Office 激活状态将会丢失。并且如果不安装新的许可证，Office 应用程序将会在第一次启动的时候报错。

## 激活步骤

### 密钥激活（联网激活）

在密钥管理中输入你的 Office 产品密钥并点击“安装密钥”，然后点击“激活”即可。

如果安装密钥时显示“找不到产品 SKU”，先安装对应的许可证，然后再试。

### 电话激活（脱机激活）

在确保安装了正确的密钥后，在密钥管理的菜单中，点击“查看安装 ID”，最后安装得到的安装 ID (CID) 即可。

如果安装密钥时显示“找不到产品 SKU”，先安装对应的许可证，然后再试。

### KMS 激活（需连接 KMS 主机）

在许可证管理中选择一个批量版 (Volume) 许可证并安装，接着在 KMS 管理中设置一个 KMS 主机，应用设置，然后点击“激活”即可。

## 查看激活信息

此功能会显示系统上已安装密钥的所有许可证的信息，包括 SKU ID、密钥信息以及许可证状态，如果是 KMS 许可证，还将会显示 KMS 主机信息等。

## 查看许可证信息

此功能会显示系统上所有许可证的信息，无论许可证是否已安装密钥。
