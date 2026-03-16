# img2img

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

img2img is a tool that uses the GPT-Image-1 model from OpenAI to generate new images from existing ones.

## Usage

Create a `.env` file with the following content:
```
OPENAI_API_KEY=****
```

### CLI

Create a single image:
```sh
deno run -A https://code4fukui.github.io/txt2img/img2img.js "render as a cute line drawing" test/Photo_of_koala_wearing_a_strawberry_hat.png
```

## Data / API

- [OpenAI API](https://platform.openai.com/docs/guides/image-generation?image-generation-model=gpt-image-1)

## License

MIT License — see [LICENSE](LICENSE).