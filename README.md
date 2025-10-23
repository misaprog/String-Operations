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

### name="the bodyGuard"

---
💡 **Tip:**
Python のインデックスは **0から始まる** ので、最初の要素はインデックス `0` にあります。

---
インデックス 6 にアクセスできます。

---
さらに、10番目のインデックスにアクセスすることもできます。

---
## Negative Indexing（負のインデックス）

Python では、文字列に **負のインデックス** を使うこともできます。
負のインデックスを使うと、文字列の **末尾から数える** ことができます。

📌 **Tip:**

```python
string = "HELLO"
print(string[-1])   # 出力: O （最後の文字）
print(string[-2])   # 出力: L （最後から2番目）
```

---

💡 **Tip:**

* `-1` → 最後の要素
* `-2` → 最後から2番目の要素

---
最初の要素はインデックス -11 で取得できます。

---
文字列の文字数はlen（長さの略）を使って調べることができます。

---
## スライス(Slicing)

スライスを使用すると、文字列から複数の文字を取得できます。0～4番目と8～12番目の要素を取得できます。

**Tip:**

スライスを取得する際、最初の数字はインデックス（0から開始）を意味し、2番目の数字はインデックスから必要な最後の要素までの長さ（1から開始）を意味します。

---
## ストライド(Stride)

ストライド値は次のように入力することもできます。「2」は、2つおきの変数を選択することを示します。

---
ストライドにスライスを組み込むこともできます。この場合、最初の5つの要素を選択し、ストライドを使用します。

---
## 文字列の連結

加算記号を使って文字列を連結（結合）することができます。その結果、両方の組み合わせからなる新しい文字列が生成されます。

---
文字列の値を複製するには、文字列に複製したい回数を掛けるだけです。この場合、回数は3です。結果は新しい文字列で、この新しい文字列は元の文字列の3つのコピーで構成されます。

---
元の変数に新しい文字列を設定することで、新しい文字列を作成できます。新しい文字列を連結すると、The BodyGuardが「The BodyGuardは最高のアルバムです」に変わる新しい文字列が生成されます。

---
## エスケープシーケンス

バックスラッシュはエスケープシーケンスの開始を表します。エスケープシーケンスは、入力が難しい可能性のある文字列を表します。例えば、バックスラッシュ「n」は改行を表します。出力は、バックスラッシュ「n」の後に改行されて表示されます。

---
同様に、バックスラッシュ「t」はタブを表します。

---
文字列にバックスラッシュを入れたい場合は、二重のバックスラッシュを使用します。

---
文字列の前に「r」を付けてバックスラッシュを表示することもできます。

---
## 文字列操作

Python には、データを操作するための文字列操作メソッドが数多くあります。ここでは、データに対していくつかの基本的な文字列操作を行ってみます。

upper メソッドを使ってみましょう。このメソッドは小文字を大文字に変換します。

---
replaceメソッドは、文字列の一部、つまり部分文字列を新しい文字列に置き換えます。置き換えたい文字列の部分を入力します。2番目の引数には、置き換えたい文字列の部分を指定します。結果は、文字列の一部が変更された新しい文字列になります。

---
find メソッドは部分文字列を検索します。引数は検索したい部分文字列で、出力はシーケンスの最初のインデックスです。部分文字列は he または Guard で見つけることができます。

---
部分文字列が文字列に含まれない場合、出力は負の値になります。例えば、文字列「Jasdfasdasdf」は部分文字列ではありません。

---
## Split メソッドは、指定された区切り文字で文字列を分割し、リストを返します。


構文

string.split(separator, maxsplit)


パラメータ

separator (オプション): 文字列を分割する区切り文字です。指定しない場合は、デフォルトの区切り文字として任意の空白文字が使用されます。

maxsplit (オプション): 分割する最大回数を指定します。指定しない場合は、分割回数に制限はありません。

戻り値: このメソッドは部分文字列のリストを返します。

---
## RegEx


Python において、RegEx (Regular Expression の略) は文字列のマッチングと処理のためのツールです。

この RegEx モジュールは、search、split、findall、sub など、正規表現を扱うための関数をいくつか提供しています。

---
## search() 関数は、文字列内の指定されたパターンを検索します。

以下は、search() 関数を使って文字列「The BodyGuard is the best」から単語「Body」を検索する方法を説明する例です。

Python には、正規表現を扱うための re という組み込みモジュールがあります。まず、re モジュールをインポートします。

---
正規表現（RegEx）は、テキスト文字列の一致や操作に使用されるパターンです。RegExには、特定の文字やパターンを一致させるために使用できる特殊なシーケンスがいくつかあります。

---
正規表現（RegEx）は、テキスト文字列の一致や操作に使用されるパターンです。RegExには、特定の文字やパターンに一致させるために使用できる特別なシーケンスがいくつかあります。

---
以下は GitHub README 用に整理・翻訳した内容です👇

---

## 🔤 Special Sequences（特殊シーケンス）

正規表現（Regular Expressions）でよく使われる **特殊シーケンス** の一覧です。
それぞれ特定の種類の文字や位置を表現するために使われます。

| **Special Sequence** | **意味（Meaning）**                     | **例（Example）**                                                                      |
| -------------------- | ----------------------------------- | ----------------------------------------------------------------------------------- |
| `\d`                 | 任意の数字文字（0〜9）にマッチ                    | `"123"` は `\d\d\d` にマッチします                                                          |
| `\D`                 | 数字以外の任意の文字にマッチ                      | `"hello"` は `\D\D\D\D\D` にマッチします                                                    |
| `\w`                 | 英数字およびアンダースコア（a-z, A-Z, 0-9, _）にマッチ | `"hello_world"` は `\w\w\w\w\w\w\w\w\w\w\w` にマッチします                                  |
| `\W`                 | 英数字・アンダースコア以外の任意の文字にマッチ             | `"@#$%"` は `\W\W\W\W` にマッチします                                                       |
| `\s`                 | 空白文字（スペース、タブ、改行など）にマッチ              | `"hello world"` は `\w\w\w\w\w\s\w\w\w\w\w` にマッチします                                  |
| `\S`                 | 空白以外の任意の文字にマッチ                      | `"hello_world"` は `\S\S\S\S\S\S\S\S\S\S\S` にマッチします                                  |
| `\b`                 | 単語と非単語の境界にマッチ                       | `"cat"` は `"The cat sat on the mat"` 内の `\bcat\b` にマッチします                           |
| `\B`                 | 単語境界 **以外** の位置にマッチ                 | `"cat"` は `"category"` 内の `\Bcat\B` にマッチします（※ `"The cat sat on the mat"` にはマッチしません） |

---

🧠 **ポイント:**
これらの特殊シーケンスは、テキストパターンを効率的に検索・抽出するために使われます。
Python では、`re` モジュールを使って正規表現を扱います。

---

## 特殊シーケンスの例:

Python コードで正規表現パターンに \d 特殊シーケンスを使用する簡単な例:

---

## Python の re モジュールでは、match.group() メソッドを使用して、正規表現パターンに一致した文字列の部分を取得します。詳細な説明は次のとおりです。

目的

一致したテキストの抽出：match.group() は、パターンに一致した部分文字列を正確に返します。
使用方法

re.search() や re.match() などの関数を使用すると、パターンが見つかった場合にマッチオブジェクトが返されます。その後、match.group() を使用して一致したテキストを取得できます。
ここで、match.group() はテキストからパターンに一致した部分文字列 1234567890 を取得します。

正規表現パターンは r"\d\d\d\d\d\d\d\d\d\d" と定義されています。これは、\d 特殊シーケンスを使用して任意の数字 (0～9) に一致させ、\d シーケンスを 10 回繰り返すことで連続する 10 桁の数字に一致させます。

---
## Python コードで正規表現パターンに \W 特殊シーケンスを使用する簡単な例:

正規表現パターンは r"\W" として定義されており、\W 特殊シーケンスを使用して単語文字（a-z、A-Z、0-9、_）以外の任意の文字に一致します。一致を検索する文字列は「Hello, world!」です。

---
## findall() 関数は、文字列内に存在する指定されたパターンをすべて検索します。

## 🔍 Using `re.findall()` to Search Strings

次の Python コードでは、文字列の中から特定のパターン（この場合は `"st"`）を検索しています。

```python
import re

s2 = "The BodyGuard is the best album of 'Whitney Houston'."

# Use the findall() function to find all occurrences of "st" in the string
result = re.findall("st", s2)

# Print out the list of matched words
print(result)
```

---

### 🧠 コードの解説

1. **`import re`**
   → Python の標準ライブラリ **`re`（regular expression：正規表現）** を読み込みます。
   正規表現は、文字列の中から特定のパターンを検索・抽出するための仕組みです。

2. **`s2 = "The BodyGuard is the best album of 'Whitney Houston'."`**
   → 検索対象となる文字列を変数 `s2` に代入しています。

3. **`re.findall("st", s2)`**
   → `findall()` 関数は、文字列 `s2` の中から **パターン `"st"`** に一致するすべての部分を探し、
   **リスト（list）形式** で返します。

   この場合、`"best"` と `"Houston"` の中に `"st"` が含まれているので、
   結果は次のようになります👇

   ```python
   ['st', 'st']
   ```

4. **`print(result)`**
   → 見つかった一致結果のリストを表示します。

---

### 💡 `result` とは？

変数 `result` は英語で「結果」という意味です。
ここでは、**`findall()` の検索結果（マッチした部分文字列の一覧）を保存するための変数**です。

つまり：

| コード                             | 意味                                        |
| ------------------------------- | ----------------------------------------- |
| `result = re.findall("st", s2)` | `"st"` に一致した部分をすべて探し、その結果を `result` に保存する |
| `print(result)`                 | 一致した結果を出力する                               |

---

### 🧾 出力結果

```python
['st', 'st']
```

🔸 `"best"` と `"Houston"` の中に `"st"` が含まれているため、
この2つの `"st"` がリストとして返されます。

---
## 正規表現のsplit()関数は、指定されたパターンに基づいて文字列を部分文字列の配列に分割します。

## ✂️ Splitting Strings with Regular Expressions

次のコードは、**文字列を空白（スペース）で分割**する方法を示しています。
ここでは Python の **`re`（正規表現）モジュール**を使用しています。

```python
import re

# Target string
s2 = "The BodyGuard is the best album of 'Whitney Houston'."

# Use the split function to split the string by the "\s"
split_array = re.split(r"\s", s2)

# The split_array contains all the substrings, split by whitespace characters
print(split_array)
```

---

### 🧠 コードの解説

1. **`import re`**
   → Python の「正規表現」モジュールを読み込みます。
   正規表現を使うことで、文字列を柔軟に検索・分割・置換できます。

2. **`s2`**
   → 操作対象となる文字列です。ここでは：

   ```
   "The BodyGuard is the best album of 'Whitney Houston'."
   ```

3. **`re.split(r"\s", s2)`**
   → `split()` 関数は、指定した**正規表現パターン**に従って文字列を分割します。

   * `\s` は「空白文字（space, tab, 改行など）」を意味します。
   * `r"\s"` の `r` は「raw string（生文字列）」を表し、`\` をそのまま扱えるようにします。

   👉つまり、「**空白文字があるところで文字列を分割**」する、という意味になります。

4. **`split_array`**
   → 分割された部分文字列のリスト（配列）が格納されます。
   例えば：

   ```python
   ['The', 'BodyGuard', 'is', 'the', 'best', 'album', 'of', "'Whitney", "Houston'."]
   ```

5. **`print(split_array)`**
   → 分割された文字列のリストを出力します。

---

### 💡 出力結果

```python
['The', 'BodyGuard', 'is', 'the', 'best', 'album', 'of', "'Whitney", "Houston'."]
```

各単語がスペース（`" "`）を区切りとしてリストの要素になっています。

---

### 🧾 ポイントまとめ

| コード要素         | 説明                                 |
| ------------- | ---------------------------------- |
| `re.split()`  | 正規表現で文字列を分割する関数                    |
| `\s`          | 空白文字（space / tab / 改行）を意味する特別なパターン |
| `r""`         | raw string 記法。`\` を特別扱いせずそのまま使用可能  |
| `split_array` | 分割結果が格納されたリスト（配列）                  |

---

## Python の正規表現の sub 関数は、文字列内のパターンの出現箇所をすべて、指定した置換文字列に置き換えるために使用されます。

## 🔁 Replacing Text in a String using Regular Expressions

このコードは、文字列の中で特定のパターン（単語やフレーズ）を**別の文字列に置き換える**方法を示しています。
Python の **`re.sub()`** 関数を使用します。

```python
import re

# Define the regular expression pattern to search for
pattern = r"Whitney Houston"

# Define the replacement string
replacement = "legend"

# Use the sub function to replace the pattern with the replacement string
new_string = re.sub(pattern, replacement, s2, flags=re.IGNORECASE)

# The new_string contains the original string with the pattern replaced by the replacement string
print(new_string)
```

---

### 🧠 コードの解説

1. **`pattern = r"Whitney Houston"`**
   → 検索したい文字列パターンを定義します。
   `r` は “raw string（生文字列）” で、正規表現内のバックスラッシュ `\` をそのまま扱うために使われます。
   この場合、 `"Whitney Houston"` という文字列を検索します。

2. **`replacement = "legend"`**
   → 置き換え後の文字列を定義します。
   見つかった `"Whitney Houston"` を `"legend"` に置き換えます。

3. **`re.sub(pattern, replacement, s2, flags=re.IGNORECASE)`**
   → `re` モジュールの **`sub()`** 関数を使用して、
   パターンにマッチした部分を置き換えます。

   **引数の意味：**

   | 引数                    | 説明                                            |
   | --------------------- | --------------------------------------------- |
   | `pattern`             | 検索する正規表現パターン                                  |
   | `replacement`         | 置き換える文字列                                      |
   | `s2`                  | 操作対象の文字列                                      |
   | `flags=re.IGNORECASE` | 大文字・小文字を区別せずに検索する設定（例：「whitney houston」でもマッチ） |

4. **`new_string`**
   → 置換が完了した新しい文字列が格納されます。
   たとえば元の文字列が：

   ```
   "The BodyGuard is the best album of 'Whitney Houston'."
   ```

   なら、置換後は：

   ```
   "The BodyGuard is the best album of 'legend'."
   ```

   となります。

5. **`print(new_string)`**
   → 置き換え後の文字列を出力します。

---

### 💡 出力結果

```python
The BodyGuard is the best album of 'legend'.
```

---

### 🧾 ポイントまとめ

| コード要素                 | 説明                             |
| --------------------- | ------------------------------ |
| `re.sub()`            | 正規表現パターンにマッチした部分を別の文字列に置き換える関数 |
| `pattern`             | 検索対象の文字列または正規表現                |
| `replacement`         | 置き換えたい文字列                      |
| `flags=re.IGNORECASE` | 大文字・小文字の違いを無視して検索するオプション       |
| `new_string`          | 置換後の新しい文字列                     |

---

🧩 **応用例**
同じ関数を使って、文中の他の単語を一括置換したり、メールアドレスや日付などのパターンを自動修正することもできます。
たとえば：

```python
re.sub(r"\d{4}-\d{2}-\d{2}", "[DATE]", text)
```

と書けば、日付（例：`2025-10-13`）を `[DATE]` に置き換えることができます。

---

## 文字列に関するクイズ

## 🧩 Quiz on Strings

### 🧠 問題

次のコードを実行したとき、各変数 `a`, `b`, `c` の値はどうなりますか？

```python
# Write your code below and press Shift+Enter to execute

a = "1"
b = "2"
c = a + b
```

---

### 🧾 解説

1. **`a = "1"`**
   → 変数 `a` に **文字列** `"1"` を代入しています。
   ※ このとき、`1` は数値ではなく文字列（str型）です。

2. **`b = "2"`**
   → 変数 `b` に **文字列** `"2"` を代入しています。
   同様に、これも数値ではなく文字列として扱われます。

3. **`c = a + b`**
   → `+` 演算子を使うと、**文字列同士は結合（concatenation）** されます。
   つまり `"1"` と `"2"` がつながって、`"12"` という新しい文字列が作られます。

---

### ✅ 結果

| 変数  | 値      | データ型       |
| --- | ------ | ---------- |
| `a` | `"1"`  | `str`（文字列） |
| `b` | `"2"`  | `str`（文字列） |
| `c` | `"12"` | `str`（文字列） |

---

### 💡 ポイント

* Python では、数値の **1 + 2 = 3** とは異なり、
  文字列 `"1" + "2"` は **結合** されて `"12"` になります。

* もし数値として計算したい場合は、`int()` 関数を使って
  **整数型（int）に変換**する必要があります。

  例：

  ```python
  c = int(a) + int(b)
  print(c)  # 出力: 3
  ```

---

### 🧩 出力例

```python
print(a)  # "1"
print(b)  # "2"
print(c)  # "12"
```

---

## 🧩 Exercise: String Slicing

### 🎯 課題

変数 `d` の最初の3文字を **スライシング（slicing）** を使って取得し、出力してください。

---

### 💻 コード例

```python
# Write your code below and press Shift+Enter to execute

d = "ABCDEFG"

# Use slicing to get the first three elements
print(d[0:3])
```

---

### 🧾 解説

* `d = "ABCDEFG"`
  → 文字列 `"ABCDEFG"` が変数 `d` に代入されています。

* `d[0:3]`
  → Python のスライス構文 `[start:end]` を使っています。
  この場合、

  * `start = 0`（最初の文字 `"A"` の位置）
  * `end = 3`（ただし、3番目のインデックス `"D"` は**含まれない**）

  よって、インデックス `0`, `1`, `2` に対応する
  `"A"`, `"B"`, `"C"` の3文字が抽出されます。

---

### ✅ 出力結果

```
ABC
```

---

### 💡 ポイント

* Python のインデックスは **0から始まる** ことを覚えておきましょう。
* スライス構文 `[0:3]` は「**0番目から2番目まで**」の意味になります。
* `d[:3]` のように **start を省略**しても同じ結果になります。

```python
print(d[:3])  # 出力: ABC
```

---
## 🧩 Exercise: String Stride（ストライド）

### 🎯 課題

変数 `e` の文字列から、**ストライド値 2** を使って、**2文字おきに** 文字を抽出して出力してください。

---

### 💻 コード例

```python
# Write your code below and press Shift+Enter to execute

e = 'clocrkr1e1c1t'

# Use stride value of 2 to get every second character
print(e[::2])
```

---

### 🧾 解説

* `e = 'clocrkr1e1c1t'`
  → 文字列 `'clocrkr1e1c1t'` が変数 `e` に代入されています。

* `e[::2]`
  → スライス構文 `[start:end:step]` を使っています。
  このとき：

  * `start`（開始位置）は省略 → 文字列の最初から開始
  * `end`（終了位置）も省略 → 最後まで
  * `step = 2` → **2文字ごとにスキップしながら**取り出す

---

### ✅ 出力結果

```
correct
```

---

### 💡 ポイント

* ストライド（`step`）は、「どの間隔で要素を選択するか」を決めます。

  * `e[::1]` → すべての文字（デフォルト）
  * `e[::2]` → 2文字おき
  * `e[::-1]` → 文字列を**逆順**にする

---
## バックスラッシュを出力します:

## 🧩 Exercise: Raw String（生文字列）

### 🎯 課題

次のコードを実行して、**バックスラッシュ（\）をそのまま出力**するようにします。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute
print(r"\\")
```

---

### 🧾 解説

* 通常、Python の文字列内では `\`（バックスラッシュ）は **エスケープシーケンス** の始まりを意味します。
  たとえば：

  * `\n` → 改行
  * `\t` → タブ

* そのため、普通の文字列 `"\\\\"` と書いた場合、
  実際の出力は `\\`（バックスラッシュ2つ）になります。

* しかし、**生文字列（raw string）** を使うと、
  Python は `\` を特別扱いせず、**そのままの文字として出力**します。

  そのため、`r"\\”` のように `r` を前に付けると：

  ```python
  print(r"\\")
  ```

  出力結果は次のようになります👇

  ```
  \\
  ```

---

### 💡 ポイント

* 文字列の前に `r` または `R` を付けると、「raw（生）文字列」として扱われます。
* 正規表現（`re` モジュール）などで多用されます。
* エスケープ処理を避けたいときに便利です。

---

✅ **まとめ**

* `r"\\”` → バックスラッシュ2つをそのまま出力。
* `r` は「raw string（生文字列）」を意味し、エスケープを無効化します。

---
## 変数 f を大文字に変換します。

## 🔤 Exercise: Convert String to Uppercase（文字列を大文字に変換）

### 🎯 課題

次のコードで、変数 `f` に代入された文字列 `"You are wrong"` を **すべて大文字に変換**します。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

f = "You are wrong"
print(f.upper())
```

---

### 🧾 解説

* Python の文字列には、**組み込みメソッド** `.upper()` があります。
  これを使うと、文字列中のすべての英字が **大文字（Uppercase）** に変換されます。

* このコードでは：

  ```python
  f = "You are wrong"
  print(f.upper())
  ```

  実行結果は以下のようになります👇

  ```
  YOU ARE WRONG
  ```

---

### 💡 ポイント

| メソッド       | 説明           | 例                                             |
| ---------- | ------------ | --------------------------------------------- |
| `.upper()` | すべて大文字に変換    | `"abc".upper()` → `"ABC"`                     |
| `.lower()` | すべて小文字に変換    | `"ABC".lower()` → `"abc"`                     |
| `.title()` | 単語の先頭を大文字に変換 | `"you are wrong".title()` → `"You Are Wrong"` |

---

✅ **まとめ**

* `.upper()` は文字列をすべて **大文字** に変換するメソッド。
* 元の文字列 `f` 自体は変更されず、変換結果が新しい文字列として返されます。
---

## 変数 f2 を小文字に変換します。

## 🔤 Exercise: Convert String to Lowercase（文字列を小文字に変換）

### 🎯 課題

次のコードで、変数 `f2` に代入された文字列 `"YOU ARE RIGHT"` を **すべて小文字に変換**します。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

f2 = "YOU ARE RIGHT"
print(f2.lower())
```

---

### 🧾 解説

* Python の文字列には **`.lower()`** というメソッドがあります。
  これを使うと、文字列中のすべての英字を **小文字（lowercase）** に変換できます。

* このコードでは：

  ```python
  f2 = "YOU ARE RIGHT"
  print(f2.lower())
  ```

  実行結果は以下のようになります👇

  ```
  you are right
  ```

---

### 💡 ポイント

| メソッド            | 説明             | 例                                    |
| --------------- | -------------- | ------------------------------------ |
| `.lower()`      | すべて小文字に変換      | `"HELLO".lower()` → `"hello"`        |
| `.upper()`      | すべて大文字に変換      | `"hello".upper()" → `"HELLO"`        |
| `.capitalize()` | 先頭の1文字だけ大文字に変換 | `"python".capitalize()" → `"Python"` |

---

✅ **まとめ**

* `.lower()` は文字列をすべて **小文字** に変換するメソッド。
* 元の文字列 `f2` はそのままで、変換後の文字列が新しく生成されます。

---
## 変数gを考え、部分文字列snowの最初のインデックスを見つける。

## 🔍 Exercise: Find the Index of a Substring（部分文字列のインデックスを検索）

### 🎯 課題

変数 `g` に格納された長い文字列の中から、部分文字列 **"snow"** が最初に現れる **インデックス位置（数値）** を見つけます。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

g = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"

# 部分文字列 "snow" の最初のインデックスを検索
index = g.find("snow")
print(index)
```

---

### 🧾 解説

* **`.find()` メソッド** は、指定した部分文字列が最初に現れる位置（インデックス）を返します。
* 文字列中で見つからない場合は **`-1`** を返します。

このコードでは：

```python
index = g.find("snow")
```

が `"snow"` の最初の出現位置を検索し、そのインデックスを `index` に格納します。

---

### 🧩 実行結果（例）

```
95
```

これは、文字列 `g` の中で `"snow"` が **95番目の位置から始まる** ことを意味します。

---

### 💡 ポイント

| メソッド                | 説明                           | 例                                    | 結果   |
| ------------------- | ---------------------------- | ------------------------------------ | ---- |
| `.find(substring)`  | 部分文字列の最初の位置を返す               | `"Hello world".find("world")`        | `6`  |
| `.rfind(substring)` | 最後に出現する位置を返す                 | `"Hello world world".rfind("world")` | `12` |
| `.index(substring)` | `.find()`と同様だが、見つからないとエラーになる | `"abc".index("a")`                   | `0`  |

---

✅ **まとめ**

* `.find()` を使うと、文字列内で特定の語句が現れる位置を簡単に特定できる。
* この例では `"snow"` が文字列中の **95番目** に現れることを確認できます。
---

## 変数 g で、部分文字列 Mary を Bob に置き換えます。

## 🔄 Exercise: Replace a Substring in a String（部分文字列の置き換え）

### 🎯 課題

変数 `g` に含まれるすべての **"Mary"** を **"Bob"** に置き換えましょう。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

g = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"

# "Mary" を "Bob" に置き換える
new_g = g.replace("Mary", "Bob")

print(new_g)
```

---

### 🧾 解説

* `.replace(old, new)` メソッドは、文字列の中の指定した部分文字列（`old`）を、別の文字列（`new`）に置き換えます。
* 元の文字列 `g` は **不変（immutable）** のため、置き換えの結果は新しい文字列として返されます。
  → そのため、結果を新しい変数 `new_g` に代入しています。

---

### 🧩 実行結果（例）

```
Bob had a little lamb Little lamb, little lamb Bob had a little lamb 
Its fleece was white as snow And everywhere that Bob went Bob went, Bob went 
Everywhere that Bob went The lamb was sure to go
```

---

### 💡 ポイント

| メソッド                     | 説明                  | 例                                     | 結果            |
| ------------------------ | ------------------- | ------------------------------------- | ------------- |
| `.replace("old", "new")` | 指定した文字列を別の文字列に置き換える | `"Hello Mary".replace("Mary", "Bob")` | `"Hello Bob"` |

---

✅ **まとめ**

* `.replace()` は文字列の置換に使用される便利なメソッドです。
* このコードでは、元の童謡の登場人物 **"Mary"** をすべて **"Bob"** に変え、新しい文字列を作成しています。
---

## 変数 g で、部分文字列 , を . に置き換えます。

## 🔄 Exercise: Replace Commas with Periods（カンマをドットに置き換える）

### 🎯 課題

変数 `g` に含まれる **`,`（カンマ）** を、すべて **`.`（ピリオド）** に置き換えましょう。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

g = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"

# カンマ (,) をドット (.) に置き換える
new_g = g.replace(",", ".")

print(new_g)
```

---

### 🧾 解説

* `.replace(old, new)` メソッドは、文字列の中の特定の部分文字列を別の文字列に置き換えるための関数です。
* この場合、**すべての「,」を「.」に変換**します。
* Python の文字列は **不変（immutable）** なので、置き換え後の新しい文字列を `new_g` に代入しています。

---

### 🧩 実行結果（例）

```
Mary had a little lamb Little lamb. little lamb Mary had a little lamb 
Its fleece was white as snow And everywhere that Mary went Mary went. Mary went 
Everywhere that Mary went The lamb was sure to go
```

---

### 💡 ポイント

| メソッド                 | 説明                  | 例                                   | 結果                |
| -------------------- | ------------------- | ----------------------------------- | ----------------- |
| `.replace(",", ".")` | 文字列中のカンマをピリオドに置き換える | `"Hello, World,".replace(",", ".")` | `"Hello. World."` |

---

✅ **まとめ**

* `.replace()` は文字列操作で頻繁に使われる基本メソッド。
* 今回は文章中の句読点を変更し、より自然な英文スタイルに整えました。
---

## 変数 g で、部分文字列をリストに分割します。

## 🧩 Exercise: Split a String into a List（文字列をリストに分割する）

### 🎯 課題

変数 `g` に格納された長い文章を、**単語ごとに分割してリスト化**しましょう。

---

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

g = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"

# 文字列をスペースで分割してリストに変換
g_list = g.split()

print(g_list)
```

---

### 🧾 解説

* `.split()` メソッドは、**文字列を指定した区切り文字（デリミタ）で分割**し、リスト（list）として返します。
* 区切り文字を指定しない場合、デフォルトで **空白（スペース）** が使用されます。
* 各単語がリストの要素として格納されます。

---

### 🧩 実行結果（例）

```
['Mary', 'had', 'a', 'little', 'lamb', 'Little', 'lamb,', 'little', 'lamb',
 'Mary', 'had', 'a', 'little', 'lamb', 'Its', 'fleece', 'was', 'white', 'as',
 'snow', 'And', 'everywhere', 'that', 'Mary', 'went', 'Mary', 'went,',
 'Mary', 'went', 'Everywhere', 'that', 'Mary', 'went', 'The', 'lamb', 'was',
 'sure', 'to', 'go']
```

---

### 💡 ポイント

| メソッド          | 説明                | 例                       | 結果                   |
| ------------- | ----------------- | ----------------------- | -------------------- |
| `.split()`    | スペースで文字列を分割してリスト化 | `"Hello world".split()` | `['Hello', 'world']` |
| `.split(",")` | カンマで文字列を分割        | `"a,b,c".split(",")`    | `['a', 'b', 'c']`    |

---

✅ **まとめ**

* `.split()` は文章やデータを扱う際の基本的な文字列操作。
* この操作で、テキストを**単語リストとして解析・処理**しやすくなります。
---

## 文字列 s3 で、\d と search() 関数を使用して数字が存在するかどうかを確認します。

## 🔍 Exercise: Check if a String Contains Numbers

**（文字列に数字が含まれているか確認する）**

### 💻 コード

```python
# Write your code below and press Shift+Enter to execute

import re  # 正規表現モジュールをインポート

s3 = "House number- 1105"

# \d は「数字（0〜9）」を表す正規表現パターン
result = re.search(r"\d", s3)

# 数字が見つかったかどうかを判定
if result:
    print("The string contains a number.")
else:
    print("No numbers found in the string.")
```

---

### 🧾 解説

* **`re.search()`**
  → 文字列全体を検索し、最初にマッチした部分を返します。
  見つからない場合は `None` を返します。

* **`\d`**
  → 数字（0〜9）のいずれか1文字にマッチします。
  つまり、「この文字列に数字が含まれているか？」を確認できます。

* **変数 `result`**
  → 一致が見つかればその情報（マッチオブジェクト）を格納します。
  → 一致しなければ `None` になります。

---

### 🧩 実行結果の例

```
The string contains a number.
```

（文字列 `"House number- 1105"` の中には数字が含まれているため）

---

### 💡 まとめ

| 関数             | 役割              |
| -------------- | --------------- |
| `re.search()`  | 最初に一致した部分を返す    |
| `re.findall()` | すべての一致をリストで返す   |
| `\d`           | 数字（digit）にマッチする |
| `\D`           | 数字以外にマッチする      |

✅ **このコードで学べるポイント**

* 正規表現の基本構文（`\d` の使い方）
* `re.search()` による文字列検索
* 検索結果を `if` 文で判定する方法

---

Python の文字列の前につける r は、

「raw（ロー）文字列」 を意味します。

### 🔹 `r` とは何か？

`r` を文字列の前につけると、
**「バックスラッシュ（\）」を特別な意味として解釈しない** という指定になります。

---

### 🔸 通常の文字列の場合

```python
print("\n")
```

これは **「改行」** を意味します。
Python は `\n` を「改行文字」として解釈してしまいます。

---

### 🔸 raw 文字列（r文字列）の場合

```python
print(r"\n")
```

これは **そのまま** 「`\n`」 と出力します。
Python は `\` を特別扱いせず、「文字」として扱います。

---

### 🔹 なぜ正規表現では `r` を使うのか？

正規表現では、`\d`, `\s`, `\w` など、
**バックスラッシュを多用** します。

もし `r` をつけないと、Python がそれらを文字列内で**別の意味（改行やタブなど）**として解釈してしまう可能性があります。

---

### ✅ 例で比較してみましょう

```python
import re
s = "Room 1105"

# rをつけない場合（非推奨）
pattern = "\\d"   # バックスラッシュを2回書かないとエラー
print(re.search(pattern, s))

# rをつける場合（推奨）
pattern = r"\d"   # そのまま1回でOK！
print(re.search(pattern, s))
```

出力結果は同じですが、
**rをつけた方が読みやすく・安全です。**

---

### 💡 まとめ

| 記号      | 意味                                |
| ------- | --------------------------------- |
| `\n`    | 改行（通常の文字列）                        |
| `r"\n"` | バックスラッシュと n をそのまま扱う（raw文字列）       |
| `r"\d"` | 数字にマッチする正規表現（Pythonが `\d` を変換しない） |

---

🔸つまり：

> **`r` は「エスケープを無効にして、正規表現をそのまま書けるようにするスイッチ」**
> ということです。
---

## 文字列 str1 で、sub() 関数を使用して部分文字列 fox を bear に置き換えます。

### 🐍 Replace a Substring Using `re.sub()`

このコードでは、Python の **正規表現モジュール（`re`）** に含まれる
`sub()` 関数を使用して、文字列の一部を別の文字列に置き換えます。

#### 🧩 コード例

```python
import re

# 元の文字列を定義
str1 = "The quick brown fox jumps over the lazy dog."

# 部分文字列 "fox" を "bear" に置き換える
new_str = re.sub("fox", "bear", str1)

# 結果を出力
print(new_str)
```

#### 🧠 コードの解説

| コード                           | 説明                                                            |
| ----------------------------- | ------------------------------------------------------------- |
| `import re`                   | 正規表現を扱う Python の標準ライブラリをインポートします。                             |
| `str1`                        | 元の文字列。ここでは「The quick brown fox jumps over the lazy dog.」です。   |
| `re.sub("fox", "bear", str1)` | `"fox"` を `"bear"` に置き換えます。`sub()` は「**substitute（置換）**」の略です。 |
| `new_str`                     | 置換後の新しい文字列が代入されます。                                            |
| `print(new_str)`              | 結果を出力します。                                                     |

#### 🧾 出力結果

```
The quick brown bear jumps over the lazy dog.
```

---

#### 💡 補足

`re.sub()` の基本構文は次の通りです：

```python
re.sub(検索パターン, 置換文字列, 対象文字列)
```

例えば：

```python
re.sub("cat", "dog", "The cat sleeps.") 
# → "The dog sleeps."
```

---

### ✅ まとめ

* `re.sub()` は **文字列の一部を置き換える関数**。
* 正規表現を使用するため、部分一致や複雑なパターンも扱えます。
* 今回の例では `"fox"` を `"bear"` に変換しました。

---

## 文字列 str2 で、findall() 関数を使用して woo のすべての出現を検索します。

### 🔍 Find All Occurrences Using `re.findall()`

このコードでは、Python の **正規表現モジュール（`re`）** に含まれる
`findall()` 関数を使って、文字列内に含まれる `"woo"` のすべての出現箇所を検索します。

#### 🧩 コード例

```python
import re

# 検索対象の文字列を定義
str2 = "How much wood would a woodchuck chuck, if a woodchuck could chuck wood?"

# findall() 関数で "woo" のすべての出現を検索
result = re.findall("woo", str2)

# 結果を出力
print(result)
```

#### 🧠 コードの解説

| コード                       | 説明                                        |
| ------------------------- | ----------------------------------------- |
| `import re`               | 正規表現（regex）モジュールをインポートします。                |
| `str2`                    | 検索対象の文字列。                                 |
| `re.findall("woo", str2)` | `"woo"` という文字列が文中に出てくるすべての箇所をリスト形式で取得します。 |
| `result`                  | 検索に一致したすべての部分文字列（"woo" のリスト）が格納されます。      |
| `print(result)`           | 一致した結果を出力します。                             |

#### 🧾 出力結果

```
['woo', 'woo', 'woo', 'woo']
```

この出力は、文字列の中で `"woo"` が **4 回** 出現していることを示しています。

---

### ✅ まとめ

* `re.findall()` は **指定したパターンに一致するすべての部分文字列をリストとして返す** 関数。
* 正規表現を使用できるため、柔軟な検索が可能。
* 今回の例では `"woo"` のすべての出現箇所を取得しました。

---

📘 **基本構文**

```python
re.findall(検索パターン, 対象文字列)
```

例：

```python
re.findall("cat", "The cat sat on the cathedral.")
# → ['cat', 'cat']
```

---






  

  










