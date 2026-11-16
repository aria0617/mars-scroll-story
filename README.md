# MARS SCROLL · 向陨石坑边缘前进

一款用滚动控制画面的火星全景互动网页。沿着毅力号的视角，探索耶泽罗陨石坑边缘。

## 体验方式

点击「进入火星横越」，向下滚动前进，向上滚动倒放。点击右侧圆点可以跳转章节，也可以使用方向键、空格、Home 和 End 键。

## 本地运行

在项目目录运行 `python3 -m http.server 8000`，访问 `http://localhost:8000`。网页使用 HTML、CSS、原生 JavaScript 和 Canvas 实现，无需安装依赖。

滚动进度映射到 120 张 WebP 图像的帧号。加载首批图像后即可进入，其余帧在后台继续加载。`index.html` 包含页面和交互逻辑，`frames/` 保存从全景图裁切出的图像。

## 影像来源

火星全景由毅力号 Mastcam-Z 拍摄，作品以此制作互动科普展示。原图为 [Perseverance Rover’s View Up Crater（PIA26373）](https://science.nasa.gov/photojournal/perseverance-rovers-view-up-crater/)，署名 NASA/JPL-Caltech/ASU/MSSS。请参照[JPL 图像使用政策](https://www.jpl.nasa.gov/jpl-image-use-policy/)使用影像。
