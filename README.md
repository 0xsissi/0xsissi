
# IISOTOP1013合约极简教程


 
### 1.  查询子合约地址 
使用`getContractsDeployed()`方法获得NFT合约地址
  ```js
      let IISOTOP1013AddrArray = new Array();
      IISOTOP1013AddrArray = await IISOTOP1013.getContractsDeployed();
      IISOTOP1013Addr = IISOTOP1013AddrArray[IISOTOP1013AddrArray.length-1];
  ```
### 2.  铸造NFT
使用`mint(address, uint) `铸造NFT


  ```js
      let  waiter = await  IISOTOP.mint(MyAddr1,5) ; //铸造5个nft
      await  waiter.wait()
  ```
### 3.  查询NFT数量
使用`balanceOf(address)`查询对应地址拥有的NFT
  ```js
      const  balance = await  IISOTOP.balanceOf(MyAddr);
  ```
