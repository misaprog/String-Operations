# String-Operations

---

## 学習目標

このラボを修了すると、以下のことができるようになります:

* 文字列 (String) を扱う
* 文字列に対して演算を行う
* インデックスやエスケープシーケンスを使って文字列を操作する

## 目次

1. 文字列とは？ (What are Strings?)
2. インデックス (Indexing)
3. 負のインデックス (Negative Indexing)
4. スライシング (Slicing)
5. ストライド (Stride)
6. 文字列の連結 (Concatenate Strings)
7. エスケープシーケンス (Escape Sequences)
8. 文字列操作 (String Manipulation Operations)
9. クイズ (Quiz on Strings)

---

## 文字列とは？ (What are Strings?)

文字列は **2つの引用符**（シングル `' '` またはダブル `" "`）で囲まれた文字の並びです。

**例:**

```python
"Hello World"
'Python Strings'
```

---
一重引用符も使えます

---
文字列はスペースと数字の組み合わせになります。

---
文字列は特殊文字の組み合わせになることもある

---
print ステートメントを使用して文字列を印刷できます。

---
文字列を別の変数にバインドまたは割り当てることができます。

---
## Indexing（インデックス）

文字列は **順序付けられたシーケンス** として考えることができます。
このシーケンスの各要素（文字）には、**インデックス（番号）** を使ってアクセスできます。

📌 **例:**

```python
string = "HELLO"
print(string[0])   # 出力: H
print(string[1])   # 出力: E
```

---

💡 **Tip:**
Python のインデックスは **0から始まる** ので、最初の要素はインデックス `0` にあります。

---



