# Alan 本地补丁

日期：2026-10-24。此分支用于备份 MaiBot 本机已使用的源码补丁，原作者与许可证保持不变。

- 上游：https://github.com/Shiroha135/GPT-SoVITS-v2-TTS-Plugin
- 安装基线：`e9a0ea566c670caf31a867f6563aae5005f0934d`
- 补丁分支：`alan-local`（以实际安装版本为基线，避免同时升级宿主或插件）
- 改动：拆分参考音频与文本语言；传入参考文本与采样参数；增加 /说、/语音、/speak 命令别名。
- 配置与数据：不上传真实运行配置、密钥、QQ 名单、聊天记录、数据库、音频、参考图库或备份文件。配置模板仅保留通用示例。
- 安装：`git clone --branch alan-local https://github.com/touching-fishfish/maibot-gpt-sovits-tts.git`，再按原 README 配置自己的服务。
- 验证：Python 源码、JSON 与 TOML 解析及凭据模式扫描；写真插件另运行现有离线测试。未发送 QQ 消息或调用付费生图/语音服务。
