-webkit-text-stroke

## 文字に輪郭線を付ける。

.title {
  -webkit-text-stroke: 2px #000;
}
2px  → 線の太さ
#000 → 線の色
-webkit-background-clip: text

## 背景を文字の形で切り抜く。
### グラデーション文字などでよく使う。

.title {
  background: linear-gradient(
    90deg,
    #ff7a7a,
    #ffd36e
  );

  -webkit-background-clip: text;
  color: transparent;
}
-webkit-text-fill-color

##文字そのものの塗り色を指定する。

.title {
  -webkit-text-fill-color: transparent;
}

###background-clip: text と組み合わせて使うことが多い。

.title {
  background: linear-gradient(
    90deg,
    #ff7a7a,
    #ffd36e
  );

  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
-webkit-line-clamp

##表示する文章の行数を制限する。

.text {
  display: -webkit-box;

  -webkit-box-orient: vertical;
  -webkit-line-clamp: 3;

  overflow: hidden;
}

この場合、
3行まで表示
↓
それ以降を省略