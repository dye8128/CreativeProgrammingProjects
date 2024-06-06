# 6/1~7

## ABC356

[提出コード](https://atcoder.jp/contests/abc356/submissions?f.Task=&f.LanguageName=&f.Status=&f.User=dye8128)

- ABCD4完
- パフォ982
- レート 1002 -> 1000 (-2)
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

## AtCoder Problems Recommendation

### ARC020 B

[提出コード](https://atcoder.jp/contests/arc020/tasks/arc020_2)

- 制約が厳しいので、使う2色とその順番について全探索できる($O(n\tiems 10^2)$)

### ABC218 E

[提出コード](https://atcoder.jp/contests/abc218/submissions/54209368)

- 報酬が低い辺から順にグラフに追加していく
  - 連結になったとき、残った辺の報酬の合計が解
  - 負の報酬の辺の存在を忘れ1WA
  - すでに連結済みの2頂点を結ぶ辺は不要であることを考えていなかったため、さらに1WA
- 実装はdsuを活用

### ABC294 B

[提出コード](https://atcoder.jp/contests/abc294/submissions/54234647)

- 日が変わる直前だったため、すぐに解けそうな問題を選択
- 文字の足し算

### ABC088 D

[提出コード](https://atcoder.jp/contests/abc088/submissions/54251906)

- 最短経路以外の白マスを全て塗れば最高スコア
  - $(H,W)$ までの最短距離を $d$, 白マスの数を $w$ とすると、$d$ が有限のとき、答えは $w-d$

### ABC296 D

[提出コード](https://atcoder.jp/contests/abc296/submissions/54281567)

- $0<a\leq \lceil\sqrt{M}\rceil$ に対して、$b = \lceil{M/a}\rceil$ を考える
- $a,b\le N$ を満たすもので最小の $ab$ を探す
  - ループ終了条件と条件判定をミスして3WA
- 計算量は $\sqrt M$
- 素因数分解問題と少し似てる？
