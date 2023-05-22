# Mononoke

A frontend engineering project documenting the journey of building a comprehensive frontend workflow from scratch

## Git 规范

git 规范包含了

- [Mononoke](#mononoke)
  - [Git 规范](#git-规范)
    - [commitlint](#commitlint)
    - [commitizen](#commitizen)
    - [husky](#husky)
    - [lint-staged](#lint-staged)
    - [conventional-changelog](#conventional-changelog)
    - [standard-version](#standard-version)
    - [gitmoji](#gitmoji)
    - [gitflow](#gitflow)
    - [代码提交规范](#代码提交规范)
      - [提交格式](#提交格式)
      - [提交类型](#提交类型)
    - [分支管理](#分支管理)
      - [主分支（Main Branch）](#主分支main-branch)
      - [发布分支（Release Branches](#发布分支release-branches)
      - [开发分支（development branch）](#开发分支development-branch)
      - [特性分支（Feature Branches）](#特性分支feature-branches)
      - [修复分支（Bugfix Branches）](#修复分支bugfix-branches)
      - [热修复分支（Hotfix Branches）](#热修复分支hotfix-branches)
      - [develop branch](#develop-branch)

### commitlint

### commitizen

### husky

### lint-staged

### conventional-changelog

### standard-version

### gitmoji

### gitflow
### 代码提交规范

#### 提交格式

```bash
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

#### 提交类型

- `feat`：新功能（feature）
- `fix`：修补 bug
- `docs`：文档（documentation）
- `style`：格式（不影响代码运行的变动）
- `refactor`：重构（即不是新增功能，也不是修改 bug 的代码变动）
- `test`：增加测试
- `chore`：构建过程或辅助工具的变动
- `revert`：回滚
- `perf`：性能优化
- `ci`：CI 配置文件修改
- `build`：打包
- `release`：版本发布
- `workflow`：工作流改动
- `types`：类型定义文件更改
- `wip`：开发中
- `config`：配置文件更改
- `deps`：依赖更新
- `BREAKING CHANGE`：破坏性变更
- `upgrade`：升级依赖
- `revert`：回滚
- `merge`：合并分支
- `init`：初始化项目
- `lint`：代码检查
- `fixup`：代码修复
- `sync`：同步代码
- `move`：移动或重命名文件
- `remove`：删除文件
- `add`：添加文件
- `update`：更新文件
- `rename`：重命名文件
- `clean`：清理文件
- `improve`：改进代码
- `perf`：性能优化
- `style`：代码格式化
  
### 分支管理

- `main`：主分支
- `release/xxx`：版本发布
- `feature/xxx`：新功能
- `bugfix/xxx`：修复 bug
- `hotfix/xxx`: 热修复线上紧急bug
- `develop`：开发分支

#### 主分支（Main Branch）

- 主分支只能从 `develop` 分支合并，不能直接修改
- 主分支只能合并到 `develop` 分支，不能直接修改
- 主分支的命名为 `main`
- 主分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签

#### 发布分支（Release Branches

- 发布分支只能从 `develop` 分支合并，不能直接修改
- 发布分支只能合并到 `develop` 分支，不能直接修改
- 发布分支的命名为 `release/xxx`
- 发布分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签
- 发布分支的生命周期：
  - 从 `develop` 分支合并
  - 合并到 `develop` 分支
  - 合并到 `main` 分支
  - 删除

#### 开发分支（development branch）

- 开发分支只能从 `develop` 分支合并，不能直接修改
- 开发分支只能合并到 `develop` 分支，不能直接修改
- 开发分支的命名为 `develop`
- 开发分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签
- 开发分支的生命周期：
  - 从 `main` 分支合并
  - 合并到 `main` 分支
  - 合并到 `release/xxx` 分支
  - 合并到 `feature/xxx` 分支
  - 合并到 `bugfix/xxx` 分支
  - 合并到 `hotfix/xxx` 分支
  - 删除
  - 保持最新
  
#### 特性分支（Feature Branches）

- 特性分支只能从 `develop` 分支合并，不能直接修改
- 特性分支只能合并到 `develop` 分支，不能直接修改
- 特性分支的命名为 `feature/xxx`
- 特性分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签
- 特性分支的生命周期：
  - 从 `develop` 分支合并
  - 合并到 `develop` 分支
  - 合并到 `main` 分支
  - 合并到 `release/xxx` 分支
  - 删除
  - 保持最新
  
#### 修复分支（Bugfix Branches）

- 修复分支只能从 `develop` 分支合并，不能直接修改
- 修复分支只能合并到 `develop` 分支，不能直接修改
- 修复分支的命名为 `bugfix/xxx`
- 修复分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签
- 修复分支的生命周期：
- 从 `develop` 分支合并
- 合并到 `develop` 分支
- 合并到 `main` 分支
- 合并到 `release/xxx` 分支
- 删除
- 保持最新

#### 热修复分支（Hotfix Branches）

- 热修复分支只能从 `main` 分支合并，不能直接修改
- 热修复分支只能合并到 `main` 分支，不能直接修改
- 热修复分支的命名为 `hotfix/xxx`
- 热修复分支的保护规则：
  - 不能直接修改
  - 不能直接推送
  - 不能直接删除
  - 不能直接强制推送
  - 不能直接强制删除
  - 不能直接强制合并
  - 不能直接强制修改
  - 不能直接强制修改历史
  - 不能直接强制修改提交
  - 不能直接强制修改标签
- 热修复分支的生命周期：
  - 从 `main` 分支合并
  - 合并到 `main` 分支
  - 合并到 `release/xxx` 分支
  - 删除
  - 保持最新

#### develop branch

<image src="./GIT 规范.svg"/>
