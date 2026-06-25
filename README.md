# 左右反転画像 生成プログラム flip.py

## 1. 概要

因数で指定した画像の左右反転画像を生成する Python 3 で動作するプログラミングです。

## 3.2. ソースコード

```python
# 子のプログラミングは python3用です。
# あらかじめ pip install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

# コマンドライン引数から入力画像と出力画像のファイル名を取得
input_image = argv[1]
output_image = argv[2]

# 画像の読み込み
img = Image.open(input_image)

# 画像の左右反転
img.flip = img.transpose(Image.FLIP_LEFT_RIGHT)

# 画像の保存
img_flip.save(output_image)
```

3.使い方

3.1.実行例

-コマンドラインフォーマット
```python
python3 flip.py <input_image_path> <output_image_path>
```

-利用例
```python
python3 flip.py input.jpg output.jpg
```

3.2.出力結果

-以下のように入力画像の左右反転画像が出力されます。
|入力画像(input.jpg)|出力画像(output.jpg)|
| --- | --- |
|<img width="1275" height="850" alt="input" src="https://github.com/user-attachments/assets/96312053-7d17-4294-8e48-515f44e92d85" />|<img width="640" height="468" alt="output" src="https://github.com/user-attachments/assets/3f4873cf-6a7f-4ccb-ab74-7821d03266d6" />|

以上
