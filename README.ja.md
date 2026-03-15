# img2img

GPT-Image-1 - OpenAIを使ったimg2imgツール。

## デモ
なし

## 機能
- 画像から新しい画像を生成することができます。

## 必要環境
- Deno

## 使い方
.envファイルを作成し、OpenAI APIキーを記載します。
```
OPENAI_API_KEY=****
```

コマンドラインから使用する例:
```sh
deno run -A https://code4fukui.github.io/txt2img/img2img.js "かわいい線画にして" test/Photo_of_koala_wearing_a_strawberry_hat.png
```

## データ・API
- [OpenAI API](https://platform.openai.com/docs/guides/image-generation?image-generation-model=gpt-image-1)

## ライセンス
MIT License