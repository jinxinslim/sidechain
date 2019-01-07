# MEET.ONE Sidechain 

## Initial accounts

```
eosio
eosio.token
eosio.msig
eosio.ram
eosio.ramfee
eosio.stake
eosio.bpay
eosio.vpay
eosio.wrap
eosio.bios
m
meetone.m
bank.m
foundation.m
```

## Initial contracts

```
eosio.system
eosio.token
eosio.msig
eosio.wrap
eosio.bios
bank.m
```

## 21 block producers

```
MEET.ONE
```

## Snapshot

get synced to the network within a minute.

## Monitor

Sidechain monitoring tool.

## Browser

Sidechain browser.

## Wallet

MEET.ONE Wallet APP.

## Governance

## Testnet

#### These are test only keys and should never be used for the production blockchain. 

Private key: EOS6MRyAjQq8ud7hVNYcfnVPJqcVpscN5So8BhtHuGYqET5GDW5CV

Public key: 5KQwrPbwdL6PhXujxW37FSSQZ1JiwsST4cqQzDeyXtP79zkvFD3


### Basic info

```
1. Core system symbol: MEETONE
2. Total supply: 10000000000.0000
```

### P2P list

```
p2p-peer-address = sidechain-test.meet.one:9876
```


### HTTPS API list

```
http://sidechain-test.meet.one:8888/v1/chain/get_info
```

### Chain info

```
{
  "chain_id": "399836e9894b222eb95063a5442069882e40abec832b89d8e3b4f4456de2bb7d"
}
```


### For Block Producers: Join blockchain network to producing

Testnet machine: 4 CPU, 16GB RAM

#### Step 1. Install
```
git clone https://github.com/meet-one/eos.git
cd eos
git checkout tags/v1.5.3
git submodule update --init --recursive
./eosio_build.sh -s MEETONE
cd build
sudo make install
echo 'PATH=$PATH:/usr/local/eosio/bin/' >> ~/.profile
source ~/.profile 
```


#### Step 2. Create new account

```
http://35.236.182.224:6677/newaccount?name=testnet115.m
```


#### Step 3. Configure the initial set of nodeos

```
1. open your config.ini 
2. replace producer-name to your producer name 
3. replace signature-provider to your produce public key and private key
4. add p2p/bnet node address
```

#### Step 4. Launch the node

```
nodeos --data-dir ./nodeos/producer-node/data-dir --config-dir ./nodeos/producer-node/config-dir --genesis-json ./nodeos/producer-node/config-dir/genesis.json
```


### For EOS Developers: [https://developers.eos.io](https://developers.eos.io)

#### Create new account

```
http://35.236.182.224:6677/newaccount?name=testnet111.m
```

#### The new account will have 1000 MEETONE token, you can get 1000 more if you want.

```
http://35.236.182.224:6677/get_token?name=testnet111.m
```


## 接入 MEET.ONE 钱包

[EOS 生态可能因此大爆发,使用门槛被极大降低](https://mp.weixin.qq.com/s/4m0ZhJP1itlhH3rabYhcAg)

[别看了，这篇是写给 EOS 应用开发者的](https://mp.weixin.qq.com/s/vZhJGP-0grJHLCOsljhZSA)
