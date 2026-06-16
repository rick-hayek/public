# Voocii 隐私政策 (Privacy Policy)

**生效日期：2026年6月13日**

欢迎使用 **账简**（以下简称“本应用”）。我们高度重视您的隐私与个人数据安全。本隐私政策旨在向您说明本应用如何收集、使用、存储及保护您的个人信息，以及您所拥有的权利。

---

## 1. 我们收集与处理的信息 (Information We Process)

本应用采用“本地优先 (Local-First)”的架构设计，除了与您自主配置的 AI 服务商进行必要的数据交互外，您的所有数据均保存在您本地设备中。

### 1.1 个人配置信息 (User Profile)
当您首次启动应用或在设置中编辑个人信息时，您可以选择提供以下信息：
- **名字（必填）**：用于在应用内为您提供个性化的称呼。
- **头像（选填）**：您可以上传照片作为头像。若未上传，应用会根据您的名字在本地生成首字母缩略头像。
- **年龄、性别、城市（选填）**：仅用于本地 AI 进行消费结构合理性分析并给出个性化财务建议。
- **存储方式**：上述所有信息均保存在您设备本地的 SQLite 数据库中。

### 1.2 交易数据与预算 (Transactions & Budgets)
- 本应用收集您手动输入或通过 AI 语音/文本解析生成的账单记录（金额、日期、分类、备注等）以及预算额度设置。
- **存储与同步方式**：上述交易和预算数据默认**仅存储在您本机的本地 SQLite 数据库中**。本应用不配置或运营任何中心化财务同步服务器。我们支持您授权将数据同步备份到您个人的 Google Drive 云端硬盘中（未来版本规划支持 iCloud 或 OneDrive 等）。该同步过程由您的设备直接与您的个人云空间建立加密连接，本应用不会传输、收集或存储您的任何数据到我们自己的服务器上。

### 1.3 语音与音频数据 (Voice & Audio)
- 当您使用“语音记账”功能时，应用会请求您的**麦克风权限**和**语音识别权限**，将您的语音流在本地或通过系统级接口转化为文本。
- **存储与传输**：转写完成的文本仅在本地处理并发送给您配置的 AI 模型，音频数据本身不会被保存或上传。

### 1.4 AI 密钥与配置 (AI API Credentials)
- 您在设置中配置的 AI 服务商信息（如 OpenAI API Key、自定义 API 接口地址、模型名称等）均以加密或安全形式保存在您本机的偏好设置中。
- **传输安全**：这些密钥仅会在您发起 AI 记账或分析时，由您的设备**直接安全地发送**给对应的 AI 服务商接口进行身份验证，绝不会途径或传输到我们的任何服务器。

---

## 2. 权限使用说明 (Device Permissions)

为了向您提供核心服务，本应用可能会在必要时向您申请以下系统权限：

| 权限名称 | 权限用途 | 拒绝影响 |
| :--- | :--- | :--- |
| **麦克风权限 (Microphone)** | 仅在您点击语音记账按钮录音时使用。 | 无法使用语音转文字记账，但仍可使用文本输入和手动记账。 |
| **语音识别 (Speech Recognition)** | 用于将您录制的语音转换为文本。 | 无法使用语音转文字记账，但仍可正常使用文本记账。 |
| **文件/相册选择 (Document/Photo Picker)** | 仅在您编辑个人头像并选择“从相册选择照片”时启动系统级选择器。 | 无法上传自定义头像照片，但仍可正常使用系统自动生成的缩略头像。本应用使用的是系统级安全选择器，**无需**您授予全局相册读取权限。 |

---

## 3. 第三方服务与数据共享 (Third-Party Services & Data Sharing)

本应用不会向任何广告商或非授权的第三方出售、共享或出租您的个人数据。数据仅在以下场景涉及网络传输或第三方交互：

1. **您配置的 AI 服务商**：
   - 当您使用 **AI 记账** 录入消费描述或请求 **AI 消费结构分析** 时，您输入的自然语言文本会被发送到您配置的 AI 供应商接口（如 OpenAI 或您自定义的 API）。
   - **请注意**：发送给 AI 服务商的仅限于与该笔交易相关的文本描述。建议您避免在交易备注或个人资料中填写极其敏感的隐私信息（如银行密码、身份证号等）。
2. **操作系统语音服务**：
   - 语音转文字（STT）可能会调用 Apple 或是 Google 系统的原生 Speech-to-Text 引擎，其数据处理遵循您设备操作系统的隐私规范。

---

## 4. 数据的控制与删除 (Your Data Control)

由于您的数据全部存储在本地，您对自己的数据拥有绝对的控制权：

- **数据导出 (Export)**：您可以在 [设置 -> 数据] 中将您的所有交易流水一键导出为 CSV 或 JSON 格式文件。
- **数据清空 (Purge & Reset)**：您可以在 [设置 -> 清空数据] 中随时一键删除所有本地账单与预算记录。
- **个人信息清除**：您可以在编辑个人信息中删除头像、年龄、性别等，或直接通过删除、卸载应用完全清除设备上的 SQLite 数据库文件。**卸载应用将不可逆地删除您所有的记账数据**，请在操作前做好数据导出备份。

---

## 5. 儿童隐私 (Children's Privacy)

本应用不以任何方式主动收集或索取儿童的个人信息。由于所有数据仅在本地留存，监护人可以通过直接管理设备或清除应用数据来控制未成年人的使用记录。

---

## 6. 隐私政策的更新 (Policy Updates)

我们可能会不时更新本隐私政策。任何更改都将直接在本页面公布，并更新本政策顶部的“生效日期”。建议您定期查看本隐私政策，以了解我们保护您隐私的最新实践。

---

## 7. 联系我们 (Contact Us)

如果您对本隐私政策或本应用的数据处理有任何疑问、建议或投诉，请通过以下方式与我们联系：

- **支持邮件**：immaxgreat@gmail.com

---

# Privacy Policy

**Effective Date: June 13, 2026**

Welcome to **Voocii** (referred to as "the App"). We are fully committed to protecting your privacy and personal data. This Privacy Policy describes how we process, use, store, and protect your information, and the rights you hold over it.

---

## 1. Information We Process

The App is designed around a **"Local-First"** architecture. Except for direct interactions with the AI provider you configure, all your data remains securely on your local device.

### 1.1 Profile Metadata
On first launch or when updating your profile in Settings, you may choose to provide:
- **Name (Required)**: To personalize greetings and prompts inside the App.
- **Avatar (Optional)**: A custom photo. If not provided, an initials avatar is generated locally.
- **Age, Gender, City (Optional)**: Used solely by the local AI context to tailor spending structure optimization advice.
- **Storage**: All profile data is saved exclusively inside your local SQLite database on your device.

### 1.2 Ledger & Budget Records
- We collect transaction logs (amount, currency, category, notes) and budget limits that you enter manually or generate via AI.
- **Storage & Synchronization**: By default, all transaction data is **stored locally on your device in a SQLite database**. We do not configure or operate any server infrastructure of our own to store or collect your financial data. We support optional user-authorized synchronization directly to your personal Google Drive cloud storage (with iCloud or OneDrive support planned for future releases). This sync establishes an encrypted connection directly between your device and your personal cloud storage; the App itself does not transmit, store, or intercept your data on any server of ours.

### 1.3 Audio & Voice Input
- When using Voice Entry, the App requests **Microphone** and **Speech Recognition** permissions to transcribe speech to text.
- **Storage & Transmission**: The converted text is sent directly to your configured AI provider. Audio recordings themselves are never recorded or stored.

### 1.4 API Keys & AI Configs
- Credentials you save (such as OpenAI API Keys or Custom Endpoint URLs) are encrypted and kept in local app preferences.
- **Transmission**: Keys are sent **directly and securely** from your device to the designated AI API endpoints for verification and are never routed through any servers of ours.

---

## 2. Permissions Explained

To deliver core features, the App requests these system permissions when needed:

| Permission | Purpose | Impact if Denied |
| :--- | :--- | :--- |
| **Microphone** | Captures audio only while you actively press the voice entry button. | Voice-to-text entry is disabled; manual text entry remains fully functional. |
| **Speech Recognition** | Converted recorded audio streams into text. | Voice-to-text entry is disabled. |
| **Document/Photo Picker** | Launches OS picker if you choose to upload a custom profile picture. | Cannot select custom photos. You will still have the hash-colored initials avatar. We use system-level pickers, meaning **no global storage/photo access permission is requested or required**. |

---

## 3. Third-Party Data Sharing

We do not sell, trade, or share your personal ledger logs with advertisers or third parties. Data exchange occurs only in these specific workflows:

1. **Your AI Provider**:
   - Natural language inputs or spending reports are sent directly to the AI service provider you configured (e.g. OpenAI) to extract records or structure advice.
   - **Recommendation**: Avoid including highly sensitive identity details (e.g. passwords, SSNs, credit card numbers) in notes or profile inputs.
2. **OS Transcription Services**:
   - Local Speech-to-Text conversion uses Apple's or Google's native speech recognition APIs, governed by their respective operating system privacy agreements.

---

## 4. Your Rights & Data Erasure

Because your data is kept 100% locally, you retain complete authority:
- **Export**: Export all transaction history to CSV/JSON under [Settings -> Data].
- **Delete All**: Purge all ledger databases anytime under [Settings -> Clear All Data].
- **App Uninstall**: Uninstalling the App deletes the local SQLite database. **This permanently and irreversibly erases all your local bookkeeping history.**

---

## 5. Children's Privacy

The App does not actively collect or solicit personal information from children in any way. As all data is stored locally, guardians can control minors' usage records by managing the device directly or clearing the app data.

---

## 6. Policy Updates

We may update this Privacy Policy from time to time. Any changes will be posted directly on this page with an updated "Effective Date" at the top. We encourage you to review this Privacy Policy periodically to stay informed about our latest privacy practices.

---

## 7. Contact Us

For questions regarding this policy or the privacy practices of this app, contact us at:

- **Support Email**: immaxgreat@gmail.com
