# img2img

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A Deno-based command-line tool for editing images using OpenAI's Image API. Provide an existing image and a text prompt to generate a new, modified version.

## Features

- **Image Editing via Prompt:** Modify existing images using simple text descriptions.
- **Flexible Input:** Accepts both local image files and remote image URLs.
- **Powered by OpenAI:** Utilizes the DALL-E 2 model via the Image Edits API endpoint.
- **Simple CLI:** Easy to use directly from your terminal.

## Requirements

- [Deno](https://deno.land/) runtime
- An OpenAI API key from the [OpenAI Platform](https://platform.openai.com/)

## Setup

1.  Create a `.env` file in the project directory with your OpenAI API key:
    ```
    OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
    ```

## Usage

Run the script from the command line, providing a text prompt and the path to an image file or a URL. The generated image will be saved as `<prompt_with_underscores>.png` in the current directory.

**Syntax:**
```sh
deno run -A ~~https://code4fukui.github.io/txt2img/img2img.js~~ *(unavailable)* "<prompt>" <image_path_or_url>
```

**Example:**

This command takes a photo of a koala and transforms it into a line drawing.

```sh
deno run -A ~~https://code4fukui.github.io/txt2img/img2img.js~~ *(unavailable)* "render as a cute line drawing" test/Photo_of_koala_wearing_a_strawberry_hat.png
```

## API Reference

This tool uses the OpenAI Images API. For more details, see the official documentation.
- [OpenAI API Reference: Image Edits](https://platform.openai.com/docs/api-reference/images/createEdit)

## License

MIT License