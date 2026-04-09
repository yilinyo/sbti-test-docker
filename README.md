# SBTI 测试（镜像）

图片和 html 已拆分。
原作者：[B站@蛆肉儿串儿](https://www.bilibili.com/video/BV1LpDHByET6/)

## Docker 运行

```bash
docker run -d -p 80:80 --name sbti-test yilin7/sbti-test
```

构建镜像：

```bash
docker build -t sbti-test .
```

启动容器：

```bash
docker run --rm -p 80:80 sbti-test
```

浏览器访问：

```text
http://localhost
```

## 说明

- 当前项目是纯静态站点，使用 `nginx` 直接托管 `index.html` 和 `image/` 目录。
- 已配置 `try_files`，直接访问站点根路径即可打开页面。
# sbti-test-docker
