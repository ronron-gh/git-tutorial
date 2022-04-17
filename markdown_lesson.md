# 1. 目次

- [1. 目次](#1-目次)
- [2. 概要](#2-概要)
- [3. 構成](#3-構成)
- [4. 機能](#4-機能)
  - [4.1. AAA](#41-aaa)
  - [4.2. BBB](#42-bbb)
  - [4.3. CCC](#43-ccc)

# 2. 概要

- 箇条書き
  - 入れ子
  - 入れ子
- 箇条書き
- 箇条書き

# 3. 構成

![基本図形](images/basic_shape.png "キャプションテキスト")

# 4. 機能


|  No.  | 機能名 | 説明   | 備考 |
| :---: | :----- | :----- | :--- |
|   1   | AAA    | ～する |      |
|   2   | BBB    | ～する |      |


  No.  | 機能名 | 説明   | 備考 
 :---: | :----- | :----- | :--- 
   1   | AAA    | ～する |      
   2   | BBB    | ～する |      
: 機能一覧

## 4.1. AAA

```mermaid
flowchart TD
    Start --> proc1([a <- status])
    proc1 --> if1{a == 0}
    if1 --yes--> proc2([異常])
    if1 --no--> proc3([正常])
    proc2 --> End
    proc3 --> End
```


## 4.2. BBB

```mermaid
stateDiagram-v2
  Initialize --> Standby: Start application
  Standby --> Manual: Manual operation
  Standby --> Auto: Execute script
  Manual --> Standby: Non operation 5min
  Auto --> Standby: Finish script


```

## 4.3. CCC

```mermaid
sequenceDiagram
  participant A as Node A
  participant B as Node B
  Note over A,B: Initial sequence
  A->>B: Request
  Note over B: Execute command
  B->>A: Responce

```