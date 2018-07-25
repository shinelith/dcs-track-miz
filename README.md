# DCS Track Miz

### 环境

* 下载安装NodeJS https://nodejs.org/en/download/

* 执行命令，完成依赖库下载

  ``` bash
  npm install
  ```

### 使用方法

* 将trk或miz文件拖到DTM目录中
* 在DTM目录空白处按Shift + 右键，选择`在此处打开Powershell窗口`
* 输入以命令，并回车

### 转换trk为miz

```bash
node dtm.js convert XXX.trk
```

### 合并trk到miz

``` bash
node dtm.js merge XXX.trk XXX.miz
```

### 清除track数据

```bash
node dtm.js clearn XXX.trk
//or
node dtm.js clearn XXX.miz
```

### 输出目录

默认在DTM中的output文件夹，可使用--output参数指定输出目录

```bash 
node dtm.js convert test.trk -o KA50
```

### 动画录制方法

* 使用任务编辑器编辑任务
* 创建多人游戏服务器，加载任务，并确保默认为暂停状态
* 调整好摄影机的位置
* 按`Pause`键，解除暂停状态，开始录制，期间所有操作会被记录
* 按`Pause`键，进入暂停状态，调整机位
* 动画录制好后退出服务器

### DCS TRK文件保存位置

TRK文件会随游戏自动保存，位置为`X:/Users/XXX/保存的游戏/DCS/Tracks/Multiplayer`

