### 容器安全

关于容器安全的课题，还在探索中。



Docker 容器逃逸案例：

1、判断是否处于docker容器里

2、配置不当引起的逃逸

- Docker Remote API 未授权访问
- docker.sock 挂载到容器内部
- docker 高危启动参数
- - privileged 特权模式
  - 挂载敏感目录
  - 相关启动参数存在的安全问题

3、Docker 软件设计引起的逃逸

- Shocker攻击
- runC容器逃逸漏洞(CVE-2019-5736)
- Docker cp 命令(CVE-2019-14271)

4、内核漏洞引起的逃逸

- 脏牛漏洞（dirtycow-docker-vdso）