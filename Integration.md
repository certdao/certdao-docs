## Integration

Integration with `certDAO` is simple. All you need to do is add a few lines of code to your wallet or interface.

The most current `certDAO` ABI is available [here](https://github.com/certdao/certdao-frontend/blob/master/src/data/certdao.json).

### Integration example

There is one main view method that you will need to call to verify that a contract is the intended contract for a given domain.

```solidity
    function verify(address contractAddress, string memory domainName)
        external
        view
        returns (bool);
```

The method takes in the contract address and the URL without the `protocol` or `www` and returns a `bool` indicating whether or not the contract is the intended contract for the given domain.

e.g `verify(0x12345678910, "certdao.net")` will return `true` if the contract is the intended contract for `certdao.net`.

There are also many view methods allowing for verification of the contract owner, the contract address, the domain name, and the registration status.

You can view them all [here](https://github.com/certdao/certdao/blob/master/contracts/interfaces/ICertDao.sol).

If you have any more questions, please reach out on discord!
