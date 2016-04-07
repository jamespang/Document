# 一. 兼容新平台

## Steps

### 前置作业
1. 驱动程式测试
2. 研究文件，开发平台与Arduino 对应平台匹配、脚位定义
3. 准备图档

### 开发作业
1. 设备型号：添加 xxx 平台
2. 设备型号：选择不同设备型号时，必须切换成相对应的平台
3. Compile API：参考Codebender，进行对应测试
4. 模块拖拉：对 Input/Output port 做防呆
5. 一键生成范例
6. Landing Page 提供下载驱动程式

### 测试作业
1. 支援模块的测试
2. Blockly 逻辑测试

# 二. 支援新模块

## Steps

### 前置作业
1. 准备图档
2. 研究文件，脚位定义
3. Arduino IDE 实测
4. 定义库
5. 定义脚本（已连接模块）
6. 定义脚本（一键生成范例）
7. 定义说明

### 开发作业
1. 分类选择：添加 xxx 模块图档
2. 添加模块metadata（脚位、脚本、说明等）

### 测试作业
1. 新支援模块的测试

# 三. Google Chrome Extension

## Steps

### 开发作业
开发 Web App
* 必须为 App 模式，Not plugin 模式
* 读取 USB port list
* Serial 写入
* Serial 读取

Frontend 使用 Post Compile API 取得 *.hex

Frontend 呼叫 Chrome Extension 进行烧录代码
