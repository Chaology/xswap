
# XSwap

### Rinkby

```
usdx token
0xaf21bb8ae7b7a5eec37964e478583cd486fd12e2

USDT:
0xA1e525F7d24D7cCB78A070BBd12C0BF21Fb4a848
USDC:
0x71abccd90dbb09c37686e4d5026c2d9597d469cb
PAX:
0xd414e78d5db39e90c704070943e067ffc0eb3d86
TUSD:
0xfeb2112e370091f25a2f96fb600484700a0ed603

DSGuard
0x93b0a865146eaddd2f0eee66b6392a5104c0fdf1

XSwap
~~0x42158a9817933a6b43b7692cb6f100275e7e7b7b~~
0x5fc6345c302d0127a777eaf924f63c028b087f56
```

### Abi

```
[ { "constant": true, "inputs": [], "name": "usdx", "outputs": [ { "name": "", "type": "address" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": true, "inputs": [], "name": "isOpen", "outputs": [ { "name": "", "type": "bool" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": false, "inputs": [], "name": "acceptOwnership", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "authority_", "type": "address" } ], "name": "setAuthority", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": true, "inputs": [], "name": "owner", "outputs": [ { "name": "", "type": "address" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": false, "inputs": [], "name": "disableOwnership", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": true, "inputs": [ { "name": "", "type": "address" } ], "name": "buyRate", "outputs": [ { "name": "", "type": "uint256" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": true, "inputs": [ { "name": "", "type": "address" } ], "name": "price", "outputs": [ { "name": "", "type": "uint256" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": true, "inputs": [ { "name": "", "type": "address" } ], "name": "sellRate", "outputs": [ { "name": "", "type": "uint256" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": true, "inputs": [], "name": "authority", "outputs": [ { "name": "", "type": "address" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": true, "inputs": [], "name": "newOwner", "outputs": [ { "name": "", "type": "address" } ], "payable": false, "stateMutability": "view", "type": "function" }, { "constant": false, "inputs": [ { "name": "newOwner_", "type": "address" } ], "name": "transferOwnership", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "inputs": [ { "name": "_usdx", "type": "address" } ], "payable": false, "stateMutability": "nonpayable", "type": "constructor" }, { "anonymous": false, "inputs": [ { "indexed": true, "name": "authority", "type": "address" } ], "name": "LogSetAuthority", "type": "event" }, { "anonymous": false, "inputs": [ { "indexed": true, "name": "owner", "type": "address" } ], "name": "LogSetOwner", "type": "event" }, { "anonymous": false, "inputs": [ { "indexed": true, "name": "owner", "type": "address" }, { "indexed": true, "name": "newOwner", "type": "address" } ], "name": "OwnerUpdate", "type": "event" }, { "constant": false, "inputs": [ { "name": "_tokenAmount", "type": "uint256" }, { "name": "_tokenAddr", "type": "address" }, { "name": "_receiver", "type": "address" } ], "name": "sellToken", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAmount", "type": "uint256" }, { "name": "_tokenAddr", "type": "address" } ], "name": "sellToken", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_usdxAmount", "type": "uint256" }, { "name": "_tokenAddr", "type": "address" }, { "name": "_receiver", "type": "address" } ], "name": "buyToken", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAmount", "type": "uint256" }, { "name": "_tokenAddr", "type": "address" } ], "name": "buyToken", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAddr", "type": "address" }, { "name": "_price", "type": "uint256" }, { "name": "_sellRate", "type": "uint256" }, { "name": "_buyRate", "type": "uint256" } ], "name": "updatePair", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAddr", "type": "address" }, { "name": "_price", "type": "uint256" } ], "name": "updatePrice", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAddr", "type": "address" }, { "name": "_sellRate", "type": "uint256" } ], "name": "updateSellRate", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAddr", "type": "address" }, { "name": "_buyRate", "type": "uint256" } ], "name": "updateBuyRate", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_open", "type": "bool" } ], "name": "emergencyStop", "outputs": [], "payable": false, "stateMutability": "nonpayable", "type": "function" }, { "constant": false, "inputs": [ { "name": "_tokenAddr", "type": "address" }, { "name": "_receiver", "type": "address" }, { "name": "_amount", "type": "uint256" } ], "name": "transferOut", "outputs": [ { "name": "", "type": "bool" } ], "payable": false, "stateMutability": "nonpayable", "type": "function" } ]
```

### run test

```
npm install
truffle test
```

### DSGuard set admin

#### permit in DSGuard.sol
```
function permit(address src, address dst, bytes32 sig)
```

#### function signature
```
"e538984f": "updateBuyRate(address,uint256)",
"9544ec58": "updatePair(address,uint256,uint256,uint256)",
"457972de": "updatePrice(address,uint256)",
"f3ceea99": "updateSellRate(address,uint256)"
```

#### functions
````
permit(${admin.address}, xswap.address, 0xe538984f)
permit(${admin.address}, xswap.address, 0x9544ec58)
permit(${admin.address}, xswap.address, 0x457972de)
permit(${admin.address}, xswap.address, 0xf3ceea99)
````
