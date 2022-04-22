
<link href="./fig_table_num.css" rel="stylesheet"></link>

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
機器構成を<a href="#ref_struct">xxx</a>に示す。

![基本図形](images/basic_shape.png "キャプションテキスト")
<p name="ref_struct" class="figure">基本図形</p>



# 4. 機能

<p class="table">テーブル見本</p>

|  No.  | 機能名 | 説明   | 備考 |
| :---: | :----- | :----- | :--- |
|   1   | AAA    | ～を<br>～する |      |
|   2   | BBB    | ～する |      |



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
<p class="figure">フローチャート</p>

## 4.2. BBB

```mermaid
stateDiagram-v2
  Initialize --> Standby: Start application
  Standby --> Manual: Manual operation
  Standby --> Auto: Execute script
  Manual --> Standby: Non operation 5min
  Auto --> Standby: Finish script


```
<p class="figure">状態遷移図</p>

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
<p class="figure">シーケンス図</p>