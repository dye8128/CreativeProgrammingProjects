# 4/27-5/3

## ABC351

[提出コード](https://atcoder.jp/contests/abc351/submissions?f.User=dye8128)

- ABC3完
- パフォ845
- レート925 -> 917 (-8)
- 前回同様、C問題までスムーズに解くことができた
- D問題の解法が思い浮かばず、E問題に挑戦するも、ACできず

### A

$\sum A_i - \sum B_i + 1$ が答え

### B

全探索して $A_{i,j}\ne B_{i,j}$となる点を見つける

### C

- 問題文通りに愚直に実装する
- ボールの大きさは全て2のべきなので、指数部分で管理する

## AtCoder Problems Recommendation

### ABC317 D

[提出コード](https://atcoder.jp/contests/abc317/submissions/53020369)

- 議席を $i$ 人とるために必要な最小鞍替え人数 $a_i$ をDPで求める
- $\min_{(\sum z_j + 1)/2}a_i$ が答えになる
- どの選挙区を高橋派が獲得したか、についての情報の持ち方に苦戦した
  - ループ順を工夫すればよかったらしい
