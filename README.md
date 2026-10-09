# 墨听音色与音效素材备份

保存音效、克隆参考音频、配套台词和可核验索引。音频按 SHA-256 去重，文件位于 `audio/前两位/完整SHA256.扩展名`；`indexes/materials.json` 记录大小、哈希与原始目录关系。

这份仓库保存参考音频材料。调用在线语音模型仍使用各插件原有的服务和账号配置；仓库不包含账号密钥、用户私有插件配置或模型权重。

- `indexes/catalogs/`：千问懒加载分组、MiMo 分组、Mossland 与火山情绪样本索引。
- `indexes/sound-libraries/`：墨听音效注册表，保留声音 ID 和变体。
- `indexes/reference-texts.json` 与 `texts/`：配套台词。
- `routes.json`：GitHub 直连与镜像候选配置。
- `tools/github_routes.js`：兼容 JRead/Rhino 的自动测速、缓存和故障回退工具。
- `tools/restore_audio.py`：下载并逐文件校验本仓库音频。

自动选路下载同一个探测文件并验证完整 SHA-256，排除返回错误网页、空文件或内容不一致的线路，再按耗时选择最快可用线路。排名定期刷新；文件读取失败会尝试下一条线路。镜像可用性取决于实际网络与服务状态。

本地完整原始素材包、下载文件、校验记录及保留账号配置的插件导入文件另外独立备份，不上传账号配置。

## 2026-10-10 原音效补全

补齐 104 个原音频文件（4,318,069 字节），对应 107 个历史原路径。

[逐项原路径、GitHub 直连和 SHA-256 对应清单](indexes/supplements/legacy-audio-20261010.json)
