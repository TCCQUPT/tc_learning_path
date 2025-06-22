# 指南介绍

在开始详细学习“docs-like-code”工作流程之前，让我们花几分钟从整体上了解一下它。

![替代文本](../assets/docs-like-code-cover-smaller-1.png){ align=left }

本指南的大部分内容来自《Docs-Like-Code》一书。我结合自己使用该工作流程的经验，对这本书做了简单的总结

本书主张将文档与开发流程紧密结合，把文档当作代码来管理。强调使用版本控制、自动化和协作的方法，同步维护文档和代码。书中通过实例展示了如何提升文档的质量、易维护性和团队合作效率，非常适合技术写作人员和开发者参考。

## 为什么要把文档当作代码来对待？

把文档视为代码，就是用开发代码的思维和方法来编写和管理文档。

那代码是怎么写和管理的呢？

大多数程序员通常按照以下流程和工具来编写和管理代码：

1. 在集成开发环境（IDE）中编辑代码，比如用 Visual Studio Code。
2. 使用代码托管平台（如 GitHub）存储和审查代码。
3. 通过 Git 分支进行协作和版本管理。
4. 在 GitHub 上跟踪问题（Issue）。
5. 使用 CI/CD 系统（如 GitHub Actions）实现自动发布。

所以，docs-like-code 方法提倡我们用和写代码一样的流程和工具来处理文档。这个工作方式高度依赖 [Git and GitHub] 这些内容将在后续章节详细介绍。

如果想了解更详细的内容和介绍，可以阅读《Docs-Like-Code》一书。本指南主要侧重于实际操作与应用。

## 指南结构

本指南通过介绍以下几个重点章节，帮助你掌握  **Docs Like Code** 工作流程。

!!!提示 

   虽然 Docs-like-code 工作流程涵盖的不仅仅是 Git 和 GitHub 等工具，但鉴于本文档篇幅有限且 GitHub 使用广泛，此处主要聚焦于 Git 和 GitHub。

1. [**Git & GitHub**](git-and-github/git-introduction.md#what-is-git)
    - 介绍: 用于版本控制的Git 和 GitHub。
    - 协作流程：拉取请求（Pull Requests）、分支管理与团队协作。
    - GitHub Desktop：简化 Git 管理的图形化界面工具。

2. [**Markdown 基础知识**](intro-to-md.md#getting-started-with-markdown)
    - 介绍：用于轻量级文档的 Markdown 语法。
    - 高级排版：表格、代码块、图表等。

3. [**Docs Like Code 工作流**](workflows/best-practice.md#a-hello-world-in-your-path-to-technical-writing)
    - 一站式工作流程：从编写到发布。
    - 真实案例：探索采用 Docs Like Code 的开源项目。
    - 实操练习：创建你的第一个拉取请求（Pull Request），体验 Docs Like Code 的“Hello World”示范

4. [**参考资料与资源**](resources.md#additional-resources)
    - 精选工具：如 Sphinx、Docusaurus 等开源选项
    - 学习资源: 技术写作课程和社区规范
    - 快速参考：高效使用的模板和速查表
