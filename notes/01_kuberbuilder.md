
# kuberbuilder 项目结构

## 1. kuberbuilder 项目初始化
安装 kuberbuilder 并初始化项目

```sh
# 1. 安装 kuberbuilder
curl -L -o kubebuilder https://go.kubebuilder.io/dl/latest/$(go env GOOS)/$(go env GOARCH)
chmod +x kubebuilder && mv kubebuilder /usr/local/bin/

# 安装 kustomize
curl -s "https://raw.githubusercontent.com/kubernetes-sigs/kustomize/master/hack/install_kustomize.sh"  | bash

# 2. 使用 kuberbuilder 初始化项目
kubebuilder init --domain tao.domain --repo github.com/hotttao/kube-learn

# 3. 使用 kuberbuilder 创建 API 
kubebuilder create api --group webapp --version v1 --kind Guestbook

```