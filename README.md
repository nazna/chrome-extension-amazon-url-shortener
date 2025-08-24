# chrome-extension-amazon-url-shortener

> Amazon URL Shortener for Google Chrome

## How to release

```sh
$ npm run release
```

## How to use

1. Download the zipped extension from [GitHub Releases](https://github.com/nazna/chrome-extension-amazon-url-shortener/releases)
2. Unzip the extension
3. Open [chrome://extensions](chrome://extensions)
4. Load the extension folder

## Notes

- Amazon は Canonical URL が存在するが、ASIN だけでなく日本語のキーワードが含まれる
- URL を共有するときに不便なので `https://amazon.co.jp/dp/${ASIN}` の形にしたい

## References

- [r7kamura/amazon_url_shortener](https://github.com/r7kamura/amazon_url_shortener)
