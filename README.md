## 公司官网

使用 Hugo 结合 GithubPages 搭建的公司官网。

目前使用 Actions 自动化构建，具体配置参看 [workflows](.github/workflows/gh-pages.yml)

## 开发调试

```shell
# 安装 hugo
brew install hugo

# clone 项目
git clone --recurse-submodules -j8 git@github.com:moerszxc/moerszxc.github.io.git
cd moerszxc.github.io

# 本地调试
hugo server -D
```

本地修改完文件后，直接在 master 分支上提交文件即可自动触发 actions 构建，构建完成后自动部署。