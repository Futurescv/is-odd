# Contributing to is-odd

感谢你愿意为 is-odd 贡献代码！这个项目很小，贡献流程也尽量简单。

## 目录

- [报告问题](#报告问题)
- [贡献代码流程](#贡献代码流程)
- [本地开发](#本地开发)
- [运行测试](#运行测试)
- [提交 PR 的规范](#提交-pr-的规范)
- [代码风格](#代码风格)

## 报告问题

如果你发现了 bug 或有新功能建议，请先到
[Issues](https://github.com/jonschlinkert/is-odd/issues) 搜索是否已有相同话题；
没有的话再 [新建 issue](https://github.com/jonschlinkert/is-odd/issues/new)。
报告 bug 时请包含：Node 版本、复现步骤、期望行为与实际行为。

## 贡献代码流程

1. **Fork** 本仓库到你自己的 GitHub 账号
2. **克隆**你的 fork 到本地：

   ```sh
   git clone https://github.com/<你的用户名>/is-odd.git
   cd is-odd
   ```

3. **新建分支**（不要直接在 master 上开发）：

   ```sh
   git checkout -b fix/my-change
   ```

4. **安装依赖并开发**（见[本地开发](#本地开发)）
5. **跑测试**，确保全部通过（见[运行测试](#运行测试)）
6. **提交并推送**：

   ```sh
   git add .
   git commit -m "fix: describe your change"
   git push origin fix/my-change
   ```

7. 在 GitHub 上向 `master` 分支发起 **Pull Request**

## 本地开发

环境要求：Node.js >= 4（建议使用 LTS 版本）。

```sh
npm install
```

核心代码只有一个文件 `index.js`，测试在 `test.js`。改动逻辑时请同步补充测试用例。

## 运行测试

测试框架使用 mocha：

```sh
npm test
```

提交 PR 前请确保本地测试全部通过，并为新逻辑添加对应测试。

## 提交 PR 的规范

- **一个 PR 只做一件事**：bug 修复和新功能请分开提交
- **提交信息**使用 conventional commits 风格：`fix:` / `feat:` / `docs:` / `test:` / `chore:`
- **保持改动最小**：不要夹带格式化、重构等与主题无关的改动
- **更新测试**：行为变化必须反映在 `test.js` 中
- **描述清楚**：PR 里说明改了什么、为什么改、如何验证

## 代码风格

- 跟随仓库现有风格（标准 JavaScript，无分号偏好以现有代码为准）
- README 由 [verb](https://github.com/verbose/verb-generate-readme) 生成，**不要直接编辑 README.md**；
  文档改动请在 `.verb.md` 模板中完成后重新生成，或先在 issue 中讨论

---

感谢你的贡献！
