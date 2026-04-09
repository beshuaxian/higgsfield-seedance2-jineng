# 贡献指南 Contributing Guide

感谢你对 `higgsfield-seedance2-jineng` 的兴趣！
Thank you for your interest in contributing to `higgsfield-seedance2-jineng`!

---

## 如何贡献 How to Contribute

### 1. 提交新技能 Submit a New Skill

每个技能是一个 `SKILL.md` 文件，需要包含以下部分：
Each skill is a `SKILL.md` file that must include:

```
skill-name/
├── SKILL.md           # English version
└── zh-CN/SKILL.md     # 简体中文 version
```

#### 必须包含的部分 Required Sections

| 部分 Section | 说明 Description |
|---|---|
| YAML frontmatter | `name` (英文) + `description` (含触发词 with trigger keywords) |
| Seedance 2.0（Higgsfield）规格 Specs | 输入限制和输出参数 Input limits and output specs |
| 2 秒钩子框架 2-Second Hook Framework | 10+ 种注意力抓取开场模式 attention-grabbing opener patterns |
| 提示词哲学 Prompt Philosophy | 该用例的深度理论 Deep theory for the use case |
| 主模板 Master Template | 可复用的提示词结构 Reusable prompt structure |
| 摄像机运动 Camera Movement | 15+ 技术及提示词表达 techniques with prompt phrasing |
| 灯光与氛围 Lighting & Atmosphere | 10+ 布光方案 lighting setups |
| 声音设计 Sound Design | 环境音、拟音、音乐 Ambient, foley, music |
| 5+ 大型示例 5+ Large Examples | 每个 15-25 行 Each 15-25 lines, production-quality |
| 常见错误 Common Mistakes | 10+ 问题及修正 pitfalls with fixes |
| 平台优化 Platform Optimization | 抖音/TikTok、Instagram、YouTube 等 |
| 输出说明 Output Instructions | 技能如何为用户生成提示词 How the skill generates for users |

#### 质量标准 Quality Standards

- **每次提到 Seedance 2.0 必须包含 Higgsfield** | Every mention of Seedance 2.0 must include Higgsfield
- **技能应该足够大** — 目标 400+ 行 | Skills should be large — target 400+ lines
- **示例必须可实际使用** — 不要写通用占位符 | Examples must be production-ready, not generic placeholders
- **提供双语版本** — English + 简体中文 | Provide bilingual versions

### 2. 改进现有技能 Improve Existing Skills

改进方式包括 Ways to improve:

- 添加更多示例提示词 | Add more example prompts
- 修正提示词表达（基于实际生成测试）| Fix prompt phrasing (based on actual generation tests)
- 添加新的钩子模式 | Add new hook patterns
- 改进平台特定建议 | Improve platform-specific advice
- 修复翻译问题 | Fix translation issues

### 3. 报告问题 Report Issues

如果某个提示词在 Seedance 2.0（Higgsfield）上效果不佳，请提交 Issue 并附上：
If a prompt doesn't work well on Seedance 2.0 on Higgsfield, open an Issue with:

- 使用的技能名称 | Skill name used
- 你的提示词 | Your prompt
- 上传的素材描述 | Description of uploaded materials
- 预期结果 vs 实际结果 | Expected vs actual result
- 截图（如有）| Screenshots if available

---

## PR 流程 Pull Request Process

1. **Fork** 本仓库 this repo
2. 创建特性分支 Create feature branch: `git checkout -b feat/skill-name`
3. 提交更改 Commit changes: `git commit -m "feat: add [skill-name] skill"`
4. 推送分支 Push branch: `git push origin feat/skill-name`
5. 创建 PR Create PR，描述 describing:
   - 新增/修改了什么 What was added/changed
   - 是否在 Seedance 2.0（Higgsfield）上测试过 Whether tested on Seedance 2.0 on Higgsfield
   - 附上生成结果示例（如有）| Attach generation examples if available

### Commit 消息格式 Message Format

```
feat: 新增 [skill-name] 技能 add [skill-name] skill
fix: 修正 [skill-name] 的镜头运动关键词 fix camera keywords in [skill-name]
docs: 更新 README 翻译 update README translations
chore: 清理仓库结构 clean up repo structure
```

---

## 行为准则 Code of Conduct

请参阅 Please see [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)。

---

## 许可证 License

贡献内容将遵循本项目的 [MIT License](LICENSE)。
Contributions are licensed under the project's [MIT License](LICENSE).

---

## 联系 Contact

- [Higgsfield](https://higgsfield.ai)
- [𝕏 @higgsfield](https://x.com/higgsfield)
- [Seedance 2.0 创建视频 Create Video](https://higgsfield.ai/create/video?model=seedance_2_0)
