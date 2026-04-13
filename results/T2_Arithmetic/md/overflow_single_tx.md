# Analysis results for /tmp/benchmark/T2_Arithmetic/overflow_single_tx.sol

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: IntegerOverflowSingleTransaction
- Function name: `underflowtostate(uint256)`
- PC address: 476
- Estimated Gas Usage: 6068 - 26163

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: /tmp/benchmark/T2_Arithmetic/overflow_single_tx.sol:30

### Code

```
count -= input
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: underflowtostate(uint256), txdata: 0x4c4f50f301, decoded_data: (452312848583266388373324160190187140051835877600158453279131187530910662656,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: IntegerOverflowSingleTransaction
- Function name: `overflowmultostate(uint256)`
- PC address: 494
- Estimated Gas Usage: 6092 - 26187

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: /tmp/benchmark/T2_Arithmetic/overflow_single_tx.sol:24

### Code

```
count *= input
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: overflowaddtostate(uint256), txdata: 0xdef92d682d, decoded_data: (20354078186246987476799587208558421302332614492007130397560903438890979819520,), value: 0x0
Caller: [ATTACKER], function: overflowmultostate(uint256), txdata: 0x5c68bc0608, decoded_data: (3618502788666131106986593281521497120414687020801267626233049500247285301248,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: IntegerOverflowSingleTransaction
- Function name: `overflowaddtostate(uint256)`
- PC address: 525
- Estimated Gas Usage: 6134 - 26229

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: /tmp/benchmark/T2_Arithmetic/overflow_single_tx.sol:18

### Code

```
count += input
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: overflowaddtostate(uint256), txdata: 0xdef92d68ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff, decoded_data: (115792089237316195423570985008687907853269984665640564039457584007913129639935,), value: 0x0


