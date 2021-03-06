# Contributing

- [Detailed CI and build process docs](../ci)
- [Our VS Code Web docs](../src/node/app)

## Development Workflow

- [VS Code prerequisites](https://github.com/Microsoft/vscode/wiki/How-to-Contribute#prerequisites)

```shell
yarn
yarn vscode
yarn watch # Visit http://localhost:8080 once completed.
```

To develop inside of an isolated docker container:

```shell
./ci/dev/container/exec.sh

root@12345:/code-server# yarn
root@12345:/code-server# yarn vscode
root@12345:/code-server# yarn watch
```

Any changes made to the source will be live reloaded.

If changes are made to the patch and you've built previously you must manually
reset VS Code then run `yarn vscode:patch`.

Some docs are available at [../src/node/app](../src/node/app) on how code-server
works internally.

## Build

- [VS Code prerequisites](https://github.com/Microsoft/vscode/wiki/How-to-Contribute#prerequisites)

```shell
yarn
yarn vscode
yarn build
yarn build:vscode
yarn release
node ./release # Run the built JavaScript with Node.
```
