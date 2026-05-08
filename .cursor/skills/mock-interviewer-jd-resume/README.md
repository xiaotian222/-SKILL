# mock-interviewer-jd-resume

基于 **JD + 简历** 的中文模拟面试 Skill（约 40 分钟）：漏斗式提问（先介绍再追问）、技术/业务约各占一半、面试后输出复盘（重点/一般问题 + 表达建议）。支持 **高级工程师 / 中级工程师**（开场问薪资，月薪 **>15000 元** 按高级）。

## 远程仓库（GitHub）

官方仓库：<https://github.com/xiaotian222/-SKILL>

克隆示例（避免本地目录名为 `-SKILL` 不好操作，可指定文件夹名）：

```bash
git clone https://github.com/xiaotian222/-SKILL.git mock-interviewer-skill
```

仓库名以 `-` 开头仅为 GitHub 允许的名称；若你本地整个「简历」项目就是该 remote 的根目录，在**项目根**执行 `git init`、`git remote add origin ...`、`git push -u origin main`（或 `master`）即可首次推送。若远程仍为**空仓库**，推送前需至少有一次 commit。

## 与本仓库的约定

在**本仓库（简历项目）根目录**维护两份材料（与 `.cursor` 同级）：

| 文件 | 说明 |
|------|------|
| `jd.md` | 目标岗位 JD：职责、要求、加分项、**薪资范围**等 |
| `resume.md` | 你的简历正文（Markdown） |

Agent 开启模拟面试时，应优先 **Read** 上述路径；若文件不存在，再请用户在对话里粘贴。

## 安装到本机 Cursor

1. 将整个文件夹 `mock-interviewer-jd-resume` 放到某项目的：

   `.cursor/skills/mock-interviewer-jd-resume/`

2. 或放到个人全局技能目录（所有项目可用）：

   `~/.cursor/skills/mock-interviewer-jd-resume/`  
   Windows 示例：`C:\Users\<用户名>\.cursor\skills\mock-interviewer-jd-resume\`

3. 确保内含：`SKILL.md`（必填）、`reference.md`（可选追问池）、本 `README.md`（说明）。

## 如何使用

1. 填好仓库根目录的 `jd.md`、`resume.md`。
2. 新开对话，**@ 技能** 选择 `mock-interviewer-jd-resume`，或说明「按 mock-interviewer-jd-resume 做模拟面试」。
3. 本 Skill 默认 `disable-model-invocation: true`，通常需**显式 @** 才会加载。
4. 按提示回答；结束后会给出《模拟面试复盘》。

## 与朋友协作优化

把本仓库（或仅 `.cursor/skills/mock-interviewer-jd-resume/` + 根目录 `jd.md` / `resume.md` 约定写进 README）用 Git 分享；对方修改 `SKILL.md` / `reference.md` 后提 PR 或互传 diff 即可。

## 文件说明

- `SKILL.md`：流程、时间、高级/中级规则、复盘模板。
- `reference.md`：追问角度池、开场确认项。
