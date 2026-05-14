# img2img

OpenAIのImage APIを使用して画像を編集するための、Denoベースのコマンドラインツールです。既存の画像とテキストプロンプトを指定することで、新しく編集された画像を生成します。

## 機能

- **プロンプトによる画像編集:** 簡単なテキストによる説明で既存の画像を変更できます。
- **柔軟な入力:** ローカルの画像ファイルとリモートの画像URLの両方に対応しています。
- **OpenAI APIの活用:** Image Edits APIエンドポイントを通じてDALL-E 2モデルを利用します。
- **シンプルなCLI:** ターミナルから直接、簡単に使用できます。

## 必須要件

- [Deno](https://deno.land/) ランタイム
- [OpenAI Platform](https://platform.openai.com/) で取得したOpenAI APIキー

## セットアップ

1. プロジェクトディレクトリに `.env` ファイルを作成し、OpenAI APIキーを設定します。
    ```
    OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
    ```

## 使い方

コマンドラインからスクリプトを実行し、テキストプロンプトと画像ファイルのパス（またはURL）を指定します。生成された画像は、現在のディレクトリに `<空白をアンダースコアに置換したプロンプト>.png` として保存されます。

**構文:**
```sh
deno run -A ~~https://code4fukui.github.io/txt2img/img2img.js~~ *(unavailable)* "<prompt>" <image_path_or_url>
```

**例:**

以下のコマンドは、コアラの写真をかわいい線画に変換します。

```sh
deno run -A ~~https://code4fukui.github.io/txt2img/img2img.js~~ *(unavailable)* "render as a cute line drawing" test/Photo_of_koala_wearing_a_strawberry_hat.png
```

## APIリファレンス

このツールはOpenAI Images APIを使用しています。詳細については、公式ドキュメントを参照してください。
- [OpenAI API Reference: Image Edits](https://platform.openai.com/docs/api-reference/images/createEdit)

## ライセンス

MIT License
