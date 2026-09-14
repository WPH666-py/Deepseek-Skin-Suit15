# JetBrains(PyCharm / WebStorm / IntelliJ)背景图

JetBrains 系 IDE 自带背景图功能, 本套件生成图片后手动导入即可。

## 1. 生成图片

```bash
python tools/wallpaper.py all --out "$HOME/DeepSkin15"
```

会得到 5 张图(2×2 拼贴 + 4 张单图):

```
grid-<宽>x<高>.jpg       2×2 拼贴
single1-<宽>x<高>.jpg    你愿意和我…吗?
single2-<宽>x<高>.jpg    DSH? DeepSeek Hentai?
single3-<宽>x<高>.jpg    你目录里的dsh是什么…大烧货吗?
single4-<宽>x<高>.jpg    正在思考…
```

想指定尺寸加 `--size 2560x1440`。

## 2. 导入

`Settings / Preferences` → `Appearance & Behavior` → `Appearance` → **Background Image** →
`+` 选择上一步的图片 → `Opacity` 建议 8%–20% → `OK`。

同一对话框里可以分别给 `Editor and tools` / `Welcome screen` / `Menus and tool windows`
设置不同图片: 例如编辑器用拼贴图, 欢迎页用单图。

## 3. 推荐搭配

- 编辑器: `grid-*.jpg`, 不透明度 10% 左右, 不遮挡代码。
- 欢迎页: 任一 `single*.jpg`, 不透明度可到 40%。
- 想换表情: 重新运行 `python tools/wallpaper.py all --out "$HOME/DeepSkin15"` 后再选另一张即可。
