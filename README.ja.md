# img2img

GPT-Image-1を利用してから画像を新しく生成するツールです。

## 使い方
`.env`ファイルを作成し、OpenAI APIキーを記載します。
```
OPENAI_API_KEY=****
```

コマンドラインから次のように使用できます:
```sh
deno run -A https://code4fukui.github.io/txt2img/img2img.js "かわいい線画にして" test/Photo_of_koala_wearing_a_strawberry_hat.png
```

## データ・API
- [OpenAI API](https://platform.openai.com/docs/guides/image-generation?image-generation-model=gpt-image-1)

## ライセンス
MIT License