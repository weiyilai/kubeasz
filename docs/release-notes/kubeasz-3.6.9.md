## kubeasz 3.6.9

kubeasz 3.6.9 发布：支持k8s v1.35 版本，组件更新和bugfix。

### 版本更新

- k8s: v1.35.4
- etcd: v3.6.7
- kubeblocks: 1.0.1
- kubernetes-dashboard: 7.14.0

### 重要更新

- 增加harbor aarch64架构离线安装包，使用circleci 自动化构建（#1510），参考：https://github.com/gjmzj/build-harbor-aarch64
- 新增自定义containerd 安装配置项，支持独立部署实例，详见：docs/blog/seperated_containerd_services_for_docker_and_k8s.md
- 优化镜像下载逻辑，失败情况下可以回退直接从指定mirror地址下载（0975932643df25）
- 修复containerd 配置非安全证书的镜像仓库（#1515）
- 优化ezdown 脚本下载二进制逻辑
- 更新国内可用的docker镜像仓库
- 修复etcd 备份恢复问题（#1516）
- 优化支持Redhat-variant Linux发行版使用dnf包管理的情况
- 新增/优化项目github 自动化流水线任务

### 文档更新

- 更新etcd 安装文档 
- 更新自定义配置部署containerd实例文档 docs/blog/seperated_containerd_services_for_docker_and_k8s.md

感谢贡献者：

wuxie0ne #1529
lswzw #1523
pansx #1519
piano-wow #1515
bookgh #1516
