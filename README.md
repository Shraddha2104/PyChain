

# Pychain
> A simple blockchain implementation in Python



## How to run:

```shell
python blockchain.py
```

## Features

* A genesis block is created with it's previous_hash as '0' and proof is assumed to be 1
* mine_block() creates a proof of work and if it satisfies the target,it will be mined.Target NONCE should have first 4 digits as 0000
* get_chain() displays all the blocks mined in json format

## Genesis block(JSON response):
```shell
{
    "chain": [
        {
            "index": 1,
            "previous_hash": "0",
            "proof": 1,
            "timestamp": "2018-06-27 09:24:10.839366"
        }
    ],
    "length": 1
}
```
## New block mined(JSON response):
```shell
{
    "index": 2,
    "message": "Congratulations, you just mined a block!",
    "previous_hash": "18ea107b497e263d2d30e706d76e082a72b0401e8443df0819728fa97459b0f4",
    "proof": 533,
    "timestamp": "2018-06-27 09:25:51.833920"
}
```
