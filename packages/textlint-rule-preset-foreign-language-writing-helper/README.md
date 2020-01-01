# @textlint-ja/textlint-rule-preset-foreign-language-writing-helper

A helper for textlint-rule-preset-foreign-language-writing 

## Install

Install with [npm](https://www.npmjs.com/):

    npm install @textlint-ja/textlint-rule-preset-foreign-language-writing-helper

## Usage

```ts
import { createKatakanaEnglishIndex } from "@textlint-ja/textlint-rule-preset-foreign-language-writing-helper";
import assert from "assert";
describe("create-katakana-english-index", () => {
    it("should should Map<カタカナ, 英単語[]>", async () => {
        const { midashiMap } = await createKatakanaEnglishIndex();
        const englishItems = midashiMap.get("エディタ");
        assert.deepStrictEqual(englishItems, ["editor"]);
    });
});

```

## Changelog

See [Releases page](https://github.com/textlint-ja/textlint-rule-preset-foreign-language-writing/releases).

## Running tests

Install devDependencies and Run `npm test`:

    npm test

## Contributing

Pull requests and stars are always welcome.

For bugs and feature requests, [please create an issue](https://github.com/textlint-ja/textlint-rule-preset-foreign-language-writing/issues).

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Author

- [github/azu](https://github.com/azu)
- [twitter/azu_re](https://twitter.com/azu_re)

## License

MIT © azu
