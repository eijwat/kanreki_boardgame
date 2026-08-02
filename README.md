# 還暦 KANREKI

**つくって祝う、六十。** — 数字カードで 60 を作りつづける、一人用のお祝い計算パズルゲーム

*A solitaire arithmetic puzzle game: keep making 60 from number cards, and celebrate.*

🎴 **Play:** ブラウザで `kanreki.html` を開くだけ / Just open `kanreki.html` in your browser

---

## 日本語

### これは何？

「還暦（かんれき）」は、60歳のお祝いをテーマにした一人用のブラウザーゲームです。0〜60 の数字が書かれた 61 枚の山札から配られる手札を、四則演算で **60** にしていきます。

### 遊び方

1. 手札はいつも 5 枚。カードと ＋ − × ÷ （ ） をタップして式を組み立てます。
2. **2〜5枚** を使って式の値がちょうど **60** になれば成功！ 使ったカードは獲得札になります。
   - 途中の計算は分数になってもかまいません（例：45 ÷ 30 × 40 = 60）。
3. 手札が減ったら、山札から 5 枚になるまで補充されます。
4. どうしても作れないときは**パス**。手札 5 枚は捨て札になり **−5点**。パスの後には「本当に作れなかったか」の答え合わせが表示されます。
5. 山札が尽きたら、残りの手札で作れるだけ作って終了です（終了ボタンは減点なし）。

### 得点

| 使った枚数 | 倍率 | 得点 |
|:---:|:---:|:---:|
| 2枚 | — | **2点** |
| 3枚 | 1.5倍 | **4.5点** |
| 4枚 | 2倍 | **8点** |
| 5枚 | 3倍 | **15点** |
| パス | — | **−5点** |

### 理論上の最高得点：180点

0〜60 の 61 枚は、「60 が作れる 5 枚組 × 12 組」＋余り 1 枚に分割できることがプログラムで実証されています。つまり最高効率の 5 枚コンボ（1枚あたり3点）で 60 枚を使い切ると **15点 × 12組 = 180点**。得点ボードにも常に表示されます。

分割例（すべて 60 になります）:

```
(35−50) × ((56−37)−23) = 60
(22+8) ÷ (29÷(41+17)) = 60
30 × ((60÷3)+(25−43)) = 60   …ほか全12組
```

### 称号

最終得点に応じて、長寿のお祝いの称号が贈られます。**60点でちょうど「祝 還暦」**！

| 得点 | 称号 |
|:---:|:---|
| 180 | 満点大還暦（百二十歳・完全制覇） |
| 160+ | 大還暦（百二十歳） |
| 140+ | 茶寿（百八歳） |
| 120+ | 白寿（九十九歳） |
| 100+ | 米寿（八十八歳） |
| 85+ | 傘寿（八十歳） |
| 70+ | 喜寿（七十七歳） |
| **60+** | **祝 還暦（六十歳）** |
| 30+ | 知命（五十歳） |
| それ未満 | 不惑（四十歳） |

### ちょっとした戦略メモ

- 手札の約 **93%** は 60 が作れます。パスする前に、もうひと粘り。
- 自動プレイのシミュレーションでは、2枚コンボ優先の手堅い戦略で平均約91点、5枚コンボ狙いで平均約97点でした。理論最高の180点までは、まだまだ上達の余地があります。
- 5枚コンボ（15点）は 2枚コンボ（2点）の 7.5 倍。大きい組み合わせを狙う勇気が高得点への道です。

### GitHub Pages

<a href="https://eijwat.github.io/kanreki_boardgame/" target="_blank">還暦ボードゲーム</a>

---

## English

### What is this?

**KANREKI** (還暦) is a solitaire browser puzzle game themed on the Japanese 60th-birthday celebration. From a 61-card deck numbered **0–60**, keep building arithmetic expressions that equal **60**.

### How to play

1. Your hand always holds 5 cards. Tap cards and + − × ÷ ( ) to build an expression.
2. Use **2–5 cards** to make exactly **60** — the used cards are yours!
   - Fractions along the way are fine (e.g. 45 ÷ 30 × 40 = 60).
3. Your hand refills to 5 from the deck.
4. Stuck? **Pass**: all 5 cards are discarded and you lose **5 points**. After passing, the game reveals whether 60 was truly impossible.
5. When the deck runs out, play what you can from your remaining hand, then end (the End button has no penalty).

### Scoring

| Cards used | Multiplier | Points |
|:---:|:---:|:---:|
| 2 | — | **2** |
| 3 | ×1.5 | **4.5** |
| 4 | ×2 | **8** |
| 5 | ×3 | **15** |
| Pass | — | **−5** |

### Theoretical maximum: 180 points

It has been verified by program that the 61 cards (0–60) can be partitioned into **twelve 5-card groups that each make 60**, with just one card left over. Using all twelve 5-card combos (the most efficient, 3 points per card) yields **15 × 12 = 180 points** — shown on the scoreboard as a reference.

### Titles

Your final score earns a Japanese longevity-celebration title. **Exactly 60 points earns "Kanreki!"** — and the ladder continues upward: Kiju (77), Sanju (80), Beiju (88), Hakuju (99), Chaju (108), all the way to **Daikanreki (120)** at 160+, and **Perfect Daikanreki** at 180.

### Strategy notes

- About **93%** of hands can make 60 — think twice before passing.
- In simulations, a cautious 2-card-first strategy averaged ~91 points and a greedy 5-card-first strategy ~97 points. The 180-point ceiling leaves plenty of room to grow.
- A 5-card combo (15 pts) is worth 7.5 times a 2-card combo (2 pts). Courage pays.

### GitHub Pages

<a href="https://eijwat.github.io/kanreki_boardgame/" target="_blank">The Kanreki Boardgame</a>

---

## 技術メモ / Technical notes

- **単一HTMLファイル（約26KB）** — ビルド不要、そのまま開くだけ / A single self-contained HTML file (~26KB), no build step
- **依存ゼロ**（Google Fonts のみ任意） / Zero dependencies (Google Fonts optional)
- **完全な有理数演算** — 式は分数のまま厳密に評価するため、丸め誤差なし / Exact rational arithmetic — expressions are evaluated as fractions, no floating-point errors
- **内蔵ソルバー** — パス時の答え合わせに、全部分集合（2〜5枚）× 全演算木を探索 / Built-in solver searches all 2–5 card subsets and operation trees for the pass check
- **日英バイリンガルUI** — ブラウザ言語を自動判定、ゲーム中いつでも切り替え可能 / Bilingual JA/EN interface with auto-detection and live toggle
