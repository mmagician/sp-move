## Integration

<!-- TODO -->


## Configuration

<!-- TODO -->


## Usage

### Client

To connect to the node you can use [polkadot.js.org/apps](https://polkadot.js.org/apps/?rpc=ws%3A%2F%2F127.0.0.1%3A9944#).

Currently additional configuration of type definitions required.
1. go to Settings tab
1. go to Developer tab
1. paste this json into:
```json
{
    "Address": "AccountId",
    "LookupSource": "AccountId"
}
```
For more about api type definitions see [docs](https://polkadot.js.org/docs/api/start/types.extend#user-defined-enum).


Then you can call extrinsics.
1. Go to Developer/Extrinsics
1. Select "mvm"
1. Select "publish" or "execute"
1. Use your modules and scripts built with [Dove][], fill arguments
1. Send signed transaction

> Dove compiler should be built with feature `ps_address`. See more [there][Dove].

[Dove]: https://github.com/dfinance/move-tools
