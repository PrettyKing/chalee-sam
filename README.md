# chalee-sam

> change log

[官网](https://aws.amazon.com/cn/serverless/sam/)

[aws sam 安装地址](https://docs.aws.amazon.com/zh_cn/serverless-application-model/latest/developerguide/install-sam-cli.html)
[aws cli 安装地址](https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/getting-started-install.html)


``` shell
# 输入你的Access Key ID、Secret Access Key、默认区域等信息。
aws configure
# AWS Access Key ID: 刚才创建的Access Key ID
# AWS Secret Access Key: 刚才创建的Secret Access Key
# Default region name: 比如 us-east-1、ap-northeast-1 等
# Default output format: 通常输入 json

# 检查你的AWS配置：
aws configure list

#设置AWS区域
aws configure set region us-east-1

# 测试
aws sts get-caller-identity
```


``` shell
# 初始化
sam init

# Template source: 选择 1 - AWS Quick Start Templates
# Package type: 选择 1 - Zip
# Runtime: 选择 nodejs20.x 或 nodejs18.x
# Architecture: 选择 x86_64 或 arm64
# Project name: 输入你的项目名称
# Quick start application: 选择模板（如 Hello World Example）

# 构建项目：
sam build

# 本地测试
sam local start-api

# 部署到AWS
sam deploy --guided

```