# 配置Limine引导程序

> **这里以在`Windows`操作系统为例**

## 下载Limine
**我们可以从[Limine Github 仓库](https://github.com/limine-bootloader/limine/releasess)下载Limine，选择合适的版本下载（一般下载`limine-binary.tar.gz`就行了，Windows可以下载`BandZip`来解压）**

## 创建项目
**新建一个文件夹，命名为你喜欢的名字，然后将你下载到`Limine`的内容解压缩到该文件夹中，注意，压缩包一般嵌套了两层同名文件夹，结构如下：**

```txt
- limine-binary/
  - limine-binary/
    - <Limine内容>

```
**记得删去一层文件夹，以便开发。在你的项目下，新建文件`limine.conf`，写入如下内容：**

```yaml
# YAML 风格，Limine 官方推荐的格式
timeout: 5
default: <你的项目名称>

/<你的项目名称>
    protocol: limine
    path: boot():/boot/<你的项目名称>.elf
```

* **前面的两处`<你的项目名称>`记得，一定要保持一致。推荐`path`处`<你的项目名称>`也与前面保持一致，方便开发，当然，也可以不一致，但是之后一定要记得修改本教程提供的[`Makefile`文件](#)**

**现在你的项目结构应当是这样的：**

```txt
├── 📁limine-binary/
│   ├── 📁 limine-tool-windows-x86
│   │   ├── 📄 limine.exe
│   ├── 📄 limine-bios-cd.bin
│   └── 📄 ... (此处省略一些文件，后面会提及)
└── limine.conf
```