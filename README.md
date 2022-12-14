# ベジェメーカー

ベジェ曲線から各座標を算出します。  

# 使い方

```js

// インスタンスを生成します。
// コンストラクタ引数には、ベジェ曲線の制御点を指定します。
const bezierInstance = new Bezier([[0, 0], [0, 1], [1, 0], [1, 1]]);

// 「calc」メソッドでベジェ曲線上の点を算出します。
bezierInstance.calc(何等分するか);

// 何等分するかについては、計算上誤差が生じる可能性があります。

```

例)

```js

// cubic-bezier(0, 1, 1, 0)
const bezierInstance = new Bezier([[0, 0], [0, 1], [1, 0], [1, 1]]);

// 「10」等分して出力
bezierInstance.calc(10);


/*
0: Array [ 0, 0 ]
1: Array [ 0.028, 0.24400000000000002 ]
2: Array [ 0.10400000000000002, 0.39200000000000007 ]
3: Array [ 0.21600000000000003, 0.468 ]
4: Array [ 0.35200000000000004, 0.496 ]
5: Array [ 0.5, 0.5 ]
6: Array [ 0.6479999999999999, 0.504 ]
7: Array [ 0.7839999999999999, 0.532 ]
8: Array [ 0.8959999999999999, 0.6079999999999999 ]
9: Array [ 0.972, 0.7559999999999998 ]
10: Array [ 1, 0.9999999999999997 ]
*/

```

