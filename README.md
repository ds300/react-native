# ts-react-native

## Mission

This is an evergreen fork of react native which patches the packager to support TypeScript
properly. It should Just Work™. If it doesn't for you, please file an issue.

This project will put out one release per stable react-native release, on an on-demand basis.
If the version you use is supported, you can simply replace the version number
for react-native in your package.json with a link to the relevant commit in this repo (see below).
Otherwise, submit an issue or a PR for the version you'd like. To see how it is done,
take a look at one of the patch commits, e.g. dd2331347d7ade1da65aff77fe85cfe7deb27d

## tsconfig.json

TypeScript code is transpiled first with TypeScript and then again as normal with Babel. Here is a good base config
to use:

```json
{
    "compilerOptions": {
        "module": "es2015",
        "moduleResolution": "node",
        "target": "es2015",
        "allowSyntheticDefaultImports": true,
        "allowJs": true,
        "jsx": "react-native",
        "noEmit": true
    }
}
```


## Supported Versions

### 0.42.3

    "react-native": "git+https://github.com/ds300/ts-react-native#dd2331347d7ade1da65aff77fe85cfe7deb27dc5",

