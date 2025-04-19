# PDF OCR 工具

这是一个基于 OCRmyPDF 的 PDF 文字识别工具，提供图形用户界面，支持中文、英文等多种语言的 OCR 处理。

## 项目结构

```
D:\OCRmyPDF_new\
├── pdf_ocr_gui.py      # GUI程序源代码
├── pdf_ocr.spec        # PyInstaller打包配置文件
├── venv/              # Python虚拟环境
└── dist/              # 打包后的可执行文件目录
    └── PDF_OCR工具.exe  # 可执行程序
```

## 环境配置

1. Python 环境：
   - Python 3.13
   - 虚拟环境位置：`D:\OCRmyPDF_new\venv`

2. 依赖软件：
   - Tesseract OCR：安装在 `D:\pdf\tesseract`
   - 已安装中文语言包

3. 主要依赖包：
   - ocrmypdf
   - tkinter
   - pyinstaller

## 功能特性

- 支持的 OCR 语言：
  - 简体中文 (chi_sim)
  - 繁体中文 (chi_tra)
  - 英文 (eng)
  - 日文 (jpn)

- OCR 处理选项：
  - 自动纠偏
  - 图像清理
  - 自动旋转
  - 多线程处理
  - PDF/A 输出

## 使用说明

1. 直接运行：
   ```cmd
   python pdf_ocr_gui.py
   ```

2. 或双击运行 `dist\PDF_OCR工具.exe`

3. 在界面中：
   - 选择输入 PDF 文件
   - 设置输出位置
   - 选择 OCR 语言
   - 配置处理选项
   - 点击"开始处理"

## 开发历史

1. 初始设置：
   - 创建虚拟环境
   - 安装 OCRmyPDF 及依赖

2. GUI 开发：
   - 创建基本界面
   - 添加文件选择功能
   - 实现 OCR 处理功能
   - 添加进度显示

3. 程序打包：
   - 使用 PyInstaller 打包
   - 配置 spec 文件
   - 生成独立可执行文件

## 注意事项

1. 确保 Tesseract 正确安装在 `D:\pdf\tesseract`
2. 运行程序前确保已安装所需的语言包
3. 处理大文件时可能需要较长时间
4. 推荐使用多线程以提高处理速度

## 下一步开发计划

1. 添加批量处理功能
2. 优化处理速度
3. 添加更多图像优化选项
4. 支持更多输出格式

## 问题排查

如果遇到问题：
1. 检查 Tesseract 安装
2. 确认语言包是否正确安装
3. 检查文件权限
4. 查看程序日志输出