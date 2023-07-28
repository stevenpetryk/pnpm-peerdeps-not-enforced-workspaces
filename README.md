# PNPM not enforcing peerDependencies in workspace packages

From [pnpm#6382](https://github.com/pnpm/pnpm/issues/6382).

## Expected behavior

`pnpm install` fails since `app` depends on `common`, which has a `webpack` peerDependency that is not satisfied by `app`'s dependencies.

## Actual behavior

`pnpm install` succeeds.
