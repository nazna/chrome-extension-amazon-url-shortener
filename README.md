# chrome-extension-amazon-url-shortener

> Amazon URL Shortener for Google Chrome

## How to release

```sh
$ npm run build
$ git tag v0.1.0
$ git push origin v0.1.0
$ gh release create v0.1.0 ./amazon-url-shortener.zip
```

## How to use

1. Download the zipped extension from [GitHub Releases](https://github.com/nazna/chrome-extension-amazon-url-shortener/releases)
2. Unzip the extension
3. Open [chrome://extensions](chrome://extensions)
4. Load the extension folder

## Notes

- Amazon は Canonical URL が存在するが、ASIN だけでなく日本語のキーワードが含まれる
- URL を共有するときに不便なので `https://amazon.co.jp/dp/${ASIN}` の形にしたい
- declarativeNetRequest API でクエリパラメータを除去する形は除去リストを用意するしかないので難しそう
  - クエリパラメータの `?` だけ残りそうだし...
  - 正規表現で ASIN を抽出する形にできるとよさそう
- 無理そうなら大人しく Content scripts でリダイレクトさせる

## References

- [r7kamura/amazon_url_shortener](https://github.com/r7kamura/amazon_url_shortener)
