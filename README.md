# ASCII Eye to Heart

[English](README_EN.md) | 简体中文

一只由字母、数字和符号构成的眼睛，在代码中苏醒。它缓缓睁开、左右环顾，镜头穿过逐渐消散的虹膜，最终抵达会跳动的爱心与闪烁的星空。

![字符眼睛变成星空与爱心的动画预览](assets/demo.gif)

*预览约为 2 倍速，实际动画会更舒缓。画面由程序逐帧生成，无需图片素材。*

## 画面里有什么

- **字符眼睛**：眼睑开合、视线移动，棕黑色虹膜带有细微纹理。
- **镜头推进**：瞳孔逐渐放大，虹膜不规则地化为字符碎片。
- **爱心与星光**：爱心渐渐成形，稳定后轻轻跳动；周围的星星各自明灭。
- **轻微信号干扰**：局部扫描错位与偶尔闪现的红色错误代码，为画面增添一点混乱感。
- **实时生成**：Python、NumPy 与 Tkinter 驱动，无需联网，也无需加载视频或图像。

## 运行

需要安装带 Tkinter 的 Python 3 和 NumPy。已经在 macOS、Python 3.14 和 NumPy 2.4 环境中运行；其他系统上的表现尚未验证。

```bash
git clone https://github.com/cgc1965565186-lab/ascii-eye-to-heart.git
cd ascii-eye-to-heart
python3 -m pip install numpy
python3 eye.py
```

在 Windows 上，可将上述命令中的 `python3` 替换为 `python` 或 `py`。Tkinter 是否随 Python 一起安装取决于你的 Python 发行版；如果报 `No module named tkinter`，请为所用 Python 安装 Tkinter。

**在 VS Code 中运行**：打开 `eye.py`，选择装有 NumPy 和 Tkinter 的 Python 解释器，然后点击右上角的运行按钮。窗口会在启动时置前；启动后可以正常切换到其他窗口。

## 控制

| 按键 | 功能 |
| --- | --- |
| `R` | 从头重播 |
| `Esc` | 关闭窗口 |

爱心成形后会继续停留，约 35 秒后开始心跳。预览经过加速，实际时间以程序播放为准。

## 技术

画面通过数学函数、纹理噪声和字符亮度映射实时生成；使用 NumPy 计算，Tkinter 绘制字符与窗口。

## 许可证

[MIT License](LICENSE)。

如果这个小作品让你会心一笑，欢迎点一颗 Star。✨
