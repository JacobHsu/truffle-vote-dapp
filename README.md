# truffle-vote-dapp

`npm install -g truffle`  
`npm install -g ethereumjs-testrpc`  
`$ testrpc`
Listening on localhost:8545

`truffle unbox react`

truffle-config.js
```js
module.exports = {
  // See <http://truffleframework.com/docs/advanced/configuration>
  // to customize your Truffle configuration!
  contracts_build_directory: path.join(__dirname, "client/src/contracts"),
  networks: {
    development: {
      host: "localhost",
      port: 8545,
      network_id: "*"
    },
    develop: {
      port: 8545
    }
  }
};
```

`truffle compile`  
`truffle migrate`  

### ganache-cli

> testrpc Error: Returned error: VM Exception while processing transaction: invalid opcode

[truffle migrate提示“VM Exception while processing transaction: invalid opcode”，合约未能部署成功](https://blog.csdn.net/qq_40467670/article/details/105468966)

使用Ganache，它也是一個以太坊客戶端，它的前身就是testrpc，用它就可以。

`$ sudo npm install ganache-cli -g`
`$ ganache-cli`

Listening on 127.0.0.1:8545

`$ cd client`
`$ npm start`

## References

[區塊鏈] 利用Truffle框架建構一個簡單的以太坊應用程式 [Part 2. Truffle box — react](https://medium.com/@cwlai.unipattern/區塊鏈-利用truffle框架建構一個簡單的以太坊應用程式-part-2-truffle-box-react-30e4de236439)  
[區塊鏈] 利用Truffle框架建構一個簡單的以太坊應用程式 [Part 1. 前置作業](https://medium.com/@cwlai.unipattern/區塊鏈-利用truffle框架建構一個簡單的以太坊應用程式-part-1-前置作業-e3014a1844f2)
