# 6/1~7

## ABC356

[提出コード](https://atcoder.jp/contests/abc356/submissions?f.Task=&f.LanguageName=&f.Status=&f.User=dye8128)

- ABCD4完
- パフォ
- レート 1002 ->
- C問題に大きく苦戦

### A

- 愚直に実装
- 0-indexed と 1-indexed がごちゃまぜになってしまい、時間がかかった

### B

- $X$ を列ごとで和をとり、 $A$ と比較

### C

- bit全探索
- bit全探索を使う方針を立てるまではよかったものの、条件分岐に大きく手間取り、5WA
  - ACまで1時間かかってしまった...

### D

$N$ 未満の整数で $i$ bit目が立っているものの個数は $$\bigg\lfloor\frac{N}{2^{i+1}}\bigg\rfloor\times2^i+\max(0,N\text{mod} 2^{i+1}-2^i)$$ であることが考察により求められる
