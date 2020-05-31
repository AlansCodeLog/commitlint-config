My preferred commitlint config.

It matches the [`@commitlint/config-conventional`](https://www.npmjs.com/package/@commitlint/config-conventional) config pretty closely, except the types are extracted straight from my semantic release config [`@alanscodelog/semantic-release-config`](https://github.com/AlansCodeLog/my-semantic-release-config) (which should be installed as a peer dependency) and the max header length is set to 100 (and that is only set to warn).


# Install
```bash
yarn add -D @alanscodelog/commitlint-config @alanscodelog/semantic-release-config
```

```json
// package.json
{
	"commitlint": { "extends": [ "@alanscodelog/commitlint-config" ] },
	// OR
	"commitlint": { "extends": [ "@alanscodelog" ] },
}
```
