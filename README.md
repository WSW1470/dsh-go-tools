# dsh-go-tools

DSH Go 本机引擎的插件包归档。

## v0.2.2

| 文件 | 说明 |
|---|---|
| `pkg-0.2.2.tgz` | 插件包（npm pack 格式） |
| `pkg-0.2.2-install.sh` | 自安装脚本 |

校验：

```
5dadd0104de604769c10077ba24e92db3441b4127fed39c4a77cd6827b7ed859  pkg-0.2.2.tgz
```

安装（DSH Go 容器内）：

```bash
mkdir -p /root/.dsh/dsh-go/plugins
cd /tmp && rm -rf pkg && mkdir pkg && cd pkg
wget -qO- https://github.com/WSW1470/dsh-go-tools/releases/download/v0.2.2/pkg-0.2.2.tgz | tar xz
cp -r package/* /root/.dsh/dsh-go/plugins/
```