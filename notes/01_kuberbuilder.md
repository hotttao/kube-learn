
# kuberbuilder 项目结构

## 1. kuberbuilder 项目初始化
安装 kuberbuilder 并初始化项目

```sh
# 1. 安装 kuberbuilder
curl -L -o kubebuilder https://go.kubebuilder.io/dl/latest/$(go env GOOS)/$(go env GOARCH)
chmod +x kubebuilder && mv kubebuilder /usr/local/bin/

# 2. 使用 kuberbuilder 初始化项目
kubebuilder init --domain tao.domain --repo github.com/hotttao/kube-learn

# 3. 使用 kuberbuilder 创建 API 
```