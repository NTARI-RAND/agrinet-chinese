# API 测试指南

## 简介
本指南说明了如何使用 curl 工具测试 Agrinet 系统中的 API 端点。

## 前置要求
- 安装了 curl 工具
- - 正在运行的 API 端点（通常在 http://localhost:8000）
  - - 测试所需的数据
   
    - ## 测试示例
   
    - ### 简单的 GET 请求
    - ```bash
      curl http://localhost:8000/api/endpoint
      ```

      ### POST 请求及数据
      ```bash
      curl -X POST http://localhost:8000/api/endpoint \
        -H "Content-Type: application/json" \
        -d '{"key": "value"}'
      ```

      ### 带身份验证的请求
      ```bash
      curl -H "Authorization: Bearer YOUR_TOKEN" \
        http://localhost:8000/api/protected
      ```

      ## 高级测试
      - 使用自定义标头
      - - 上传文件
        - - 处理错误响应
         
          - ## 总结
          - 使用 curl 可以高效且轻松地测试所有 API 端点。
          - 
