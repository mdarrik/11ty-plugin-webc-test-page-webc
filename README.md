# Demo webc newline html stripping

This is a quick demo of how a newline after the front matter in a webc page component strips the `<!DOCTYPE html>` and `<html lang="en">` elements off of the rendered output.

It's a pretty bare-bones 11ty site with a single `index.webc` page.

To build it follow these steps:

1. In your terminal, run `npm install`
2. Run `npm run build`
3. Look at the output file in `_site/index.html`. With `"@11ty/eleventy": "^2.0.0-canary.23"` and `"@11ty/eleventy-plugin-webc": "^0.8.1"`, the output should be missing the `html` declarations.

## Example output

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test</title>
  </head>
  <body>
    <h1>Hi, this is a test</h1>
  

</body>
</html>
```
