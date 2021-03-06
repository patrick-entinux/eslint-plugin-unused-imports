# eslint-plugin-unused-imports

Find and remove unused es6 modules

## Typescript

If running [typescript-eslint](https://github.com/typescript-eslint/typescript-eslint) please use the `-ts`
extension on your rules to make this also leverage type information (otherwise the autofixer will remove
imports only used for type information).

## Installation

You'll first need to install [ESLint](http://eslint.org):

```
$ npm i eslint --save-dev
```

Next, install `eslint-plugin-unused-imports`:

```
$ npm install eslint-plugin-unused-imports --save-dev
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-unused-imports` globally.

## Usage

Add `unused-imports` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
	"plugins": ["unused-imports"]
}
```

Then configure the rules you want to use under the rules section.

e.g.

```json
{
	"rules": {
		"no-unused-vars": "off",
		"unused-imports/no-unused-imports": 2,
		"unused-imports/no-unused-vars": 1
	}
}
```

## Supported Rules

- `no-unused-imports`
- `no-unused-vars`
- `no-unused-imports-ts`
- `no-unused-vars-ts`
