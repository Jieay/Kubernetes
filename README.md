# Kubernetes

## 在 Docker Hub 上进行 Github 授权。
2.1 打开 帐号的 "Account Settings" ，点击 "Linked Accounts"。
2.2 在Github 后面点击 "Connect" 进行相关账户的授权

## 在 Docker Hub 上创建仓库。
2.3 点击页面上方的 "Repositories" ,进入到仓库管理页面。
2.4 在点击 "Create Repository" ，在name 栏中输入仓库名称 "kube-apiserver"(建议使用组件名称作为仓库名称)。
2.5 在 Build Settings 选项点击 github 的图标，选择GitHub帐号和仓库。这里选择 k8s-images 仓库，即上面步骤中创建的仓库。
2.6 点击 Build Rules，会出现构建规则选项卡。在Docker Tag 选项输入版本号 v1.18.3 ，在Dockerfile location 选项卡中输入Github 中创建的文件名称 kube-apiserver:v1.18.3，然后点击 Create & Build。
注：Dockerfile location 选项必须要与Github 中文件名称对应上。
2.7 在此仓库的 Builds 页面查看创建进度。
2.8 在 Recent Builds 中可以查看构建详情，状态变成 success 后就可以进行下载。


