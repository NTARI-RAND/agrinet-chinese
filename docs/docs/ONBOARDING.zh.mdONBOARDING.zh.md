# 新手入门指南

## 简介
本指南说明了如何设置新节点以连接到 Agrinet 分布式网络。

## 前置要求
- Python 3.8 或更高版本
- - 访问 Agrinet 主服务器
  - - 新节点的 IP 地址
   
    - ## 设置步骤
   
    - ### 1. 基本安装
    - ```bash
      pip install agrinet
      agrinet-cli init
      ```

      ### 2. 集成设置
      编辑配置文件：
      ```yaml
      node:
        name: "my-node"
        public_ip: "192.168.1.100"
        port: 8000
      ```

      ### 3. 连接到网络
      ```bash
      agrinet-cli connect --server http://main-server:8000
      ```

      ## 验证设置
      ```bash
      agrinet-cli status
      ```

      ## 故障排除
      - 检查节点的健康状态
      - - 确保与其他节点的连接
        - - 监控日志中的错误
         
          - ## 支持
          - 如需帮助，请参阅官方文档或联系支持团队。
          - 
