<div align="center">
=================================================================
<h1>Python Training・パイソン研修</h1>
<p style="font-size: 25px; font-weight: bold;">
  <strong>Date:</strong> 10/2025
</p>
<p style="font-size: 25px; font-weight: bold;">
  <strong>Moderator:</strong> Daniel.J.Q.Goh
</p>
=================================================================
</div>

# 変数

問題１
次の⽂章のうち正しいものには○を、正しくないものには×をつけてください。

**回答:**
（1） コンピュータは、Pythonのプログラムコードを直接理解して処理を⾏う。 **×**
   - Pythonコードはインタープリターによって機械語に変換されてから実行される

（2） Pythonのプログラムコードは、大⽂字と小⽂字の違いを区別しない。 **×**
   - Pythonは大文字と小文字を区別する（case-sensitive）

（3） Pythonには、1⾏ずつプログラムコードを⼊⼒して、そのつど実⾏する⽅法がある。 **○**
   - 対話型モード（REPL: Read-Eval-Print Loop）が利用可能

（4） 「 print(こんにちは)」と記述すると、「こんにちは」という⽂字列が出⼒される。 **×**
   - 文字列は引用符で囲む必要がある：`print("こんにちは")`

（5） 変数には後から異なる値を代⼊できる **○**
   - Pythonの変数は可変（mutable）で、異なる値を再代入可能

<br>

---

<br>

問題 2 not sure <br> 
次の⽂章の空欄に⼊れるべき語句を、選択肢から選んでください。
コンピュータが値を記憶しておくための⼊れ物のことを[（1）]という。
[（1）] に値を格納することを[（2） ]という。
[（2）] を⾏うには、記号[（3）]を使⽤する。
[（1）]に[（2）]された値は print 関数を⽤いてコンソールに[（4）] できる。
【選択肢】
・代⼊ ・変数 ・オブジェクト ・出⼒
・>>> ・=

**回答:**
- （1）**変数**
- （2）**代入**  
- （3）**=**
- （4）**出力**

**完成した文章:**
コンピュータが値を記憶しておくための⼊れ物のことを**変数**という。
**変数**に値を格納することを**代入**という。
**代入**を⾏うには、記号**=**を使⽤する。
**変数**に**代入**された値は print 関数を⽤いてコンソールに**出力**できる。

**例:**
```python
# 変数nameに文字列を代入
name = "Python"
# 変数の値を出力
print(name)  # Python と出力される
```

<br>

---

<br>

問題 3
対話モードで、次の計算を実⾏して結果を確認しましょう。<br>
（1） 1 + 2 + 3 + 4 <br>
（2） 2 + 3 * 2 <br>
（3） (2 + 3) * 2 <br>
（4） 10 / 2.5 <br>
（5） 3 / 0 <br>

**Python print文での実行:**

```python
# （1） 1 + 2 + 3 + 4
print("(1) 1 + 2 + 3 + 4 =", 1 + 2 + 3 + 4)
# 結果: 10

# （2） 2 + 3 * 2
print("(2) 2 + 3 * 2 =", 2 + 3 * 2)
# 結果: 8 (掛け算が先に計算される)

# （3） (2 + 3) * 2
print("(3) (2 + 3) * 2 =", (2 + 3) * 2)
# 結果: 10 (括弧内が先に計算される)

# （4） 10 / 2.5
print("(4) 10 / 2.5 =", 10 / 2.5)
# 結果: 4.0 (小数点付きの結果)

# （5） 3 / 0
try:
    print("(5) 3 / 0 =", 3 / 0)
except ZeroDivisionError as e:
    print("(5) 3 / 0 = エラー:", e)
# 結果: ZeroDivisionError (ゼロ除算エラー)
```

**実行結果:**
```
(1) 1 + 2 + 3 + 4 = 10
(2) 2 + 3 * 2 = 8
(3) (2 + 3) * 2 = 10
(4) 10 / 2.5 = 4.0
(5) 3 / 0 = エラー: division by zero
```

**ポイント:**
- 演算子の優先順位: `*` や `/` は `+` や `-` より先に計算される
- 括弧を使うと計算順序を変更できる
- ゼロで割るとエラーが発生する

<br>

---

<br>

問題 4 <br>
次のようにして、インタラクティブシェルで変数aに10という値を代⼊し、print関数で値を出⼒できます。<br>
（1） 変数bに5という値を代⼊してから、print関数で変数bに代⼊された値を 出⼒してください。<br>
（2） 変数cに「Python」という⽂字列を代⼊してから、print関数で変数cに 代⼊された値を出⼒してください

**回答:**

**例として与えられた変数aの場合:**
```python
>>> a = 10
>>> print(a)
10
```

**（1） 変数bに5を代入して出力:**
```python
>>> b = 5
>>> print(b)
5
```

**（2） 変数cに「Python」を代入して出力:**
```python
>>> c = "Python"
>>> print(c)
Python
```

**まとめて実行する場合:**
```python
# 変数の代入
a = 10
b = 5
c = "Python"

# 変数の出力
print("a =", a)  # a = 10
print("b =", b)  # b = 5
print("c =", c)  # c = Python
```

**実行結果:**
```
a = 10
b = 5
c = Python
```

**ポイント:**
- 数値は引用符なしで代入: `b = 5`
- 文字列は引用符で囲んで代入: `c = "Python"`
- `print()`関数で変数の値を出力できる

<br>

--- 

<br>

問題５<br>
変数に関する問題です。<br>
（1） 整数型の変数xに100を代⼊して、その値を画⾯出⼒してください。<br>
（2） ⽂字列型の変数nameに’tarou’を代⼊して、
その値を画⾯出⼒してください。<br>
（3） 実数型の変数piに3.14を代⼊して、その値を画⾯出⼒してください。
変数に関する問題です。<br>
（1） 整数型の変数xに100を代⼊して、その値を画⾯出⼒してください。<br>
（2） ⽂字列型の変数nameに'tarou'を代⼊して、
その値を画⾯出⼒してください。<br>
（3） 実数型の変数piに3.14を代⼊して、その値を画⾯出⼒してください。

**回答:**

**（1） 整数型の変数x:**
```python
x = 100
print(x)
```

**（2） 文字列型の変数name:**
```python
name = 'tarou'
print(name)
```

**（3） 実数型の変数pi:**
```python
pi = 3.14
print(pi)
```

**まとめて実行:**
```python
# 変数の代入
x = 100        # 整数型
name = 'tarou' # 文字列型
pi = 3.14      # 実数型

# 値の出力
print(x)
print(name)
print(pi)
```

**実行結果:**
```
100
tarou
3.14
```

<br>

---

<br>

# 演算子

問題 1 <br>
以下の記述について、正しいものには○を、誤りのあるものには×をつけてくだ
さい。<br>
（1） 一度int型の値を代⼊した変数aに対して、後から⽂字列を代⼊することは
できない。<br>
（2） int型の値とfloat型の値を加算するときには、その前にint型の値をfloat型
に型変換しておく必要がある。<br>
（3） int型とfloat型の値を含む算術演算の結果はfloat型になる。<br>
（4） a = int(3.8)と記述した場合、変数aの値は4になる<br>

**回答:**

（1） 一度int型の値を代⼊した変数aに対して、後から⽂字列を代⼊することはできない。 **×**
   - Pythonは動的型付け言語のため、変数の型は実行時に決定され、異なる型の値を再代入可能
   ```python
   a = 10        # int型
   a = "hello"   # str型に変更可能
   ```

（2） int型の値とfloat型の値を加算するときには、その前にint型の値をfloat型に型変換しておく必要がある。 **×**
   - Pythonは自動的に型変換（暗黙の型変換）を行う
   ```python
   result = 5 + 3.14  # 自動的にfloat型になる（8.14）
   ```

（3） int型とfloat型の値を含む算術演算の結果はfloat型になる。 **○**
   - 異なる数値型の演算では、より精度の高い型（float）に自動変換される
   ```python
   print(5 + 3.0)    # 8.0 (float型)
   print(10 / 2)     # 5.0 (float型)
   ```

（4） a = int(3.8)と記述した場合、変数aの値は4になる **×**
   - `int()`関数は小数点以下を切り捨て（truncate）するため、3になる
   ```python
   a = int(3.8)   # a = 3 (切り捨て)
   a = int(3.2)   # a = 3 (切り捨て)
   # 四捨五入したい場合は round() を使用
   a = round(3.8) # a = 4
   ```

**補足説明:**
```python
# 型変換の例
x = 10        # int
y = 3.14      # float
z = x + y     # 13.14 (float型)

# 明示的な型変換
a = float(5)  # 5.0
b = int(3.9)  # 3 (切り捨て)
c = str(123)  # "123"
```

<br>

---

<br>

問題 2
次の値を求める式を書いてください。
（1） 100を9で割った商
（2） 1000を7で割った余り
（3） 3の5乗

**回答:**

**（1） 100を9で割った商:**
```python
# 整数除算演算子 // を使用
quotient = 100 // 9
print("100を9で割った商:", quotient)
# 結果: 11
```

**（2） 1000を7で割った余り:**
```python
# 剰余演算子 % を使用
remainder = 1000 % 7
print("1000を7で割った余り:", remainder)
# 結果: 6
```

**（3） 3の5乗:**
```python
# べき乗演算子 ** を使用
power = 3 ** 5
print("3の5乗:", power)
# 結果: 243
```

**まとめて実行:**
```python
# 各種演算の実行
quotient = 100 // 9    # 商（整数除算）
remainder = 1000 % 7   # 余り（剰余）
power = 3 ** 5         # べき乗

# 結果の出力
print("(1) 100 ÷ 9 の商:", quotient)
print("(2) 1000 ÷ 7 の余り:", remainder)
print("(3) 3の5乗:", power)

# 検算
print("検算: 9 × 11 + 1 =", 9 * 11 + 1)  # 100
print("検算: 7 × 142 + 6 =", 7 * 142 + 6)  # 1000
```

**実行結果:**
```
(1) 100 ÷ 9 の商: 11
(2) 1000 ÷ 7 の余り: 6
(3) 3の5乗: 243
検算: 9 × 11 + 1 = 100
検算: 7 × 142 + 6 = 1000
```

**Pythonの算術演算子:**
- `//` : 整数除算（商を求める）
- `%` : 剰余演算（余りを求める）
- `**` : べき乗
- `/` : 通常の除算（小数点も含む結果）

<br>

---

<br>

問題 3 <br>
次の命令⽂を、加算代⼊（+=）、減算代⼊（-=）、乗算代⼊（*=）、除算代⼊（/=）、剰余代⼊（%=）の演算子を使って、短い表現に書き換えてください。<br>
（1） a = a + 5 <br>
（2） b = b – 6 <br>
（3） c = c * a <br>
（4） d = d / 3 <br>
（5） e = e % 2 <br>

**回答:**

**（1） a = a + 5**
```python
# 元の表現
a = a + 5
# 短い表現（加算代入）
a += 5
```

**（2） b = b – 6**
```python
# 元の表現
b = b - 6
# 短い表現（減算代入）
b -= 6
```

**（3） c = c * a**
```python
# 元の表現
c = c * a
# 短い表現（乗算代入）
c *= a
```

**（4） d = d / 3**
```python
# 元の表現
d = d / 3
# 短い表現（除算代入）
d /= 3
```

**（5） e = e % 2**
```python
# 元の表現
e = e % 2
# 短い表現（剰余代入）
e %= 2
```

**実際の使用例:**
```python
# 初期値を設定
a = 10
b = 20
c = 3
d = 15
e = 7

print("初期値:")
print(f"a = {a}, b = {b}, c = {c}, d = {d}, e = {e}")

# 複合代入演算子を使用
a += 5    # a = a + 5 → 15
b -= 6    # b = b - 6 → 14
c *= a    # c = c * a → 3 * 15 = 45
d /= 3    # d = d / 3 → 15 / 3 = 5.0
e %= 2    # e = e % 2 → 7 % 2 = 1

print("計算後:")
print(f"a = {a}, b = {b}, c = {c}, d = {d}, e = {e}")
```

**実行結果:**
```
初期値:
a = 10, b = 20, c = 3, d = 15, e = 7
計算後:
a = 15, b = 14, c = 45, d = 5.0, e = 1
```

**複合代入演算子一覧:**
- `+=` : 加算代入（a += 5 は a = a + 5 と同じ）
- `-=` : 減算代入（b -= 6 は b = b - 6 と同じ）
- `*=` : 乗算代入（c *= a は c = c * a と同じ）
- `/=` : 除算代入（d /= 3 は d = d / 3 と同じ）
- `%=` : 剰余代入（e %= 2 は e = e % 2 と同じ）
- `**=` : べき乗代入（x **= 2 は x = x ** 2 と同じ）
- `//=` : 整数除算代入（y //= 3 は y = y // 3 と同じ）

<br>

---

<br>

# ⽂字列とリスト
問題 １<br>
次のプログラムコードを実⾏した後の変数aの値を答えてください（対話
モードで実⾏するときに表⽰されるプロンプト「>>>」は省略しています）。<br>
（1） a = 3 <br>
　　　a *= 3 <br>
（2） b = 2 <br>
　　　a = b * b <br>
（3） a = int(1.9) <br>
（4） x = 'XXX' <br>

y = 'YYY'　　a = x + y

**回答:**

**（1） a = 3, a *= 3**
```python
a = 3     # aに3を代入
a *= 3    # a = a * 3 → 3 * 3 = 9
print(a)  # 9
```
**変数aの値: 9**

**（2） b = 2, a = b * b**
```python
b = 2     # bに2を代入
a = b * b # a = 2 * 2 = 4
print(a)  # 4
```
**変数aの値: 4**

**（3） a = int(1.9)**
```python
a = int(1.9)  # 小数点以下切り捨て → 1
print(a)      # 1
```
**変数aの値: 1**

**（4） x = 'XXX', y = 'YYY', a = x + y**
```python
x = 'XXX'   # xに文字列'XXX'を代入
y = 'YYY'   # yに文字列'YYY'を代入
a = x + y   # 文字列の連結 → 'XXX' + 'YYY' = 'XXXYYY'
print(a)    # XXXYYY
```
**変数aの値: 'XXXYYY'**

**実際の実行例:**
```python
# (1)の実行
a = 3
a *= 3
print("(1) a =", a)  # (1) a = 9

# (2)の実行  
b = 2
a = b * b
print("(2) a =", a)  # (2) a = 4

# (3)の実行
a = int(1.9)
print("(3) a =", a)  # (3) a = 1

# (4)の実行
x = 'XXX'
y = 'YYY'
a = x + y
print("(4) a =", a)  # (4) a = XXXYYY
```

**実行結果:**
```
(1) a = 9
(2) a = 4
(3) a = 1
(4) a = XXXYYY
```

**ポイント:**
- `*=` は乗算代入演算子
- `int()` 関数は小数点以下を切り捨て
- 文字列の `+` 演算子は文字列の連結を行う

<br>

---

<br>

問題2
「私は21歳です。」という⽂字列が出⼒されるように作成し
た次のプログラムコードは、実⾏するとエラーが発生します。
適切に動作するように修正してください。

```python
age = 21
print('私は' + age + '歳です。')
```

**回答:**

**エラーの原因:**
```python
age = 21
print('私は' + age + '歳です。')
# TypeError: can only concatenate str (not "int") to str
```
- `age`は整数型(int)で、文字列と直接連結できないためエラーが発生

**修正方法（3つの解決策）:**

**方法1: str()関数を使用して型変換**
```python
age = 21
print('私は' + str(age) + '歳です。')
```

**方法2: f-string（フォーマット済み文字列リテラル）を使用**
```python
age = 21
print(f'私は{age}歳です。')
```

**方法3: format()メソッドを使用**
```python
age = 21
print('私は{}歳です。'.format(age))
```

**方法4: printの複数引数を使用**
```python
age = 21
print('私は', age, '歳です。', sep='')
```

**実行結果（すべて同じ出力）:**
```
私は21歳です。
```

**推奨解決策の比較:**
```python
age = 21

# 最も推奨される方法（Python 3.6以降）
print(f'私は{age}歳です。')

# 従来の方法（わかりやすい）
print('私は' + str(age) + '歳です。')

# より複雑な文字列操作に適している
print('私は{}歳です。'.format(age))
```

**ポイント:**
- Pythonでは異なるデータ型を直接連結できない
- 数値を文字列と連結する場合は型変換が必要
- f-stringが最も読みやすく効率的（Python 3.6以降推奨）
- `str()`関数で明示的に文字列に変換するのも良い方法

<br>

---

<br>

問題 ３
リスト [1,2,3] のすべての要素を画⾯上に表⽰してください。

**回答:**

**簡単な回答**
```python
a = [1,2,3]
print(a)
```

**実行結果**
[1, 2, 3]

**他の表示方法も紹介します:**

**方法1: 直接リストを表示（最も簡単）**
```python
my_list = [1, 2, 3]
print(my_list)
# 出力: [1, 2, 3]
```

**方法2: forループで各要素を個別に表示**
```python
my_list = [1, 2, 3]
for element in my_list:
    print(element)
# 出力:
# 1
# 2
# 3
```

**方法3: forループで横一列に表示**
```python
my_list = [1, 2, 3]
for element in my_list:
    print(element, end=' ')
print()  # 改行
# 出力: 1 2 3
```

**方法4: unpacking演算子（*）を使用**
```python
my_list = [1, 2, 3]
print(*my_list)
# 出力: 1 2 3
```

**方法5: join()メソッドで文字列として表示**
```python
my_list = [1, 2, 3]
print(' '.join(map(str, my_list)))
# 出力: 1 2 3
```

**実行結果の比較:**
```python
my_list = [1, 2, 3]

print("方法1:", my_list)           # [1, 2, 3]
print("方法4:", *my_list)          # 1 2 3
print("方法5:", ' '.join(map(str, my_list)))  # 1 2 3
```

**ポイント:**
- あなたの解答は**完全に正解**です
- `print(list)`でリスト全体を表示できる
- 用途に応じて異なる表示方法を選択可能
- 括弧付きで表示したい場合は`print(list)`
- 要素だけを表示したい場合は`print(*list)`

<br>

---

<br>

# モジュール

問題 1<br>
mathモジュールを利⽤して、cos(120°)の値を求めてください。<br>
**Python標準ライブラリmathを使用してcos(120°)を計算**

```python
import math

# 120度をラジアンに変換してcos値を計算
angle_degrees = 120
angle_radians = math.radians(angle_degrees)
cos_value = math.cos(angle_radians)

print(f"cos({angle_degrees}°) = {cos_value}")
```

**実行結果:**
```
cos(120°) = -0.5
```

**詳細説明:**
```python
import math

# 方法1: degrees → radians → cos
degrees = 120
radians = math.radians(degrees)  # 120° を ラジアンに変換
result = math.cos(radians)       # cosine値を計算
print(f"cos(120°) = {result}")   # -0.5

# 方法2: 直接ラジアン値を使用
# 120° = 2π/3 ラジアン
radians_direct = 2 * math.pi / 3
result2 = math.cos(radians_direct)
print(f"cos(2π/3) = {result2}")  # -0.5

# 方法3: math.piを使って計算
result3 = math.cos(math.pi * 2/3)
print(f"cos(2π/3) = {result3}")  # -0.5

# 数学的確認
print(f"120° = {math.radians(120)} ラジアン")
print(f"2π/3 = {2 * math.pi / 3} ラジアン")
```

**重要なポイント:**
- Python の `math.cos()` は**ラジアン**を引数として受け取る
- 度をラジアンに変換: `math.radians(degrees)`
- ラジアンを度に変換: `math.degrees(radians)`
- cos(120°) = cos(2π/3) = -0.5

**その他の三角関数例:**
```python
import math

angle = 120  # 度

# 三角関数の計算
cos_val = math.cos(math.radians(angle))
sin_val = math.sin(math.radians(angle))
tan_val = math.tan(math.radians(angle))

print(f"sin({angle}°) = {sin_val:.6f}")    # ≈ 0.866025
print(f"cos({angle}°) = {cos_val:.6f}")    # = -0.5
print(f"tan({angle}°) = {tan_val:.6f}")    # ≈ -1.732051
```

<br>

---

<br>

問題 2 <br>
mathモジュールを利⽤して、81の平⽅根を求めてください。<br>

**回答:**

```python
import math

# 81の平方根を計算
number = 81
square_root = math.sqrt(number)

print(f"{number}の平方根 = {square_root}")
```

**実行結果:**
```
81の平方根 = 9.0
```

**詳細説明:**
```python
import math

# 方法1: math.sqrt()を使用（最も一般的）
result1 = math.sqrt(81)
print(f"math.sqrt(81) = {result1}")  # 9.0

# 方法2: べき乗演算子を使用
result2 = 81 ** 0.5
print(f"81 ** 0.5 = {result2}")      # 9.0

# 方法3: pow()関数を使用
result3 = pow(81, 0.5)
print(f"pow(81, 0.5) = {result3}")   # 9.0

# 方法4: math.pow()を使用
result4 = math.pow(81, 0.5)
print(f"math.pow(81, 0.5) = {result4}")  # 9.0

# 検証: 9² = 81
verification = 9 ** 2
print(f"検証: 9² = {verification}")  # 81
```

**実行結果:**
```
math.sqrt(81) = 9.0
81 ** 0.5 = 9.0
pow(81, 0.5) = 9.0
math.pow(81, 0.5) = 9.0
検証: 9² = 81
```

**その他の平方根の例:**
```python
import math

# 様々な数値の平方根
numbers = [4, 9, 16, 25, 36, 49, 64, 81, 100]

print("数値\t平方根")
print("-" * 15)
for num in numbers:
    sqrt_val = math.sqrt(num)
    print(f"{num}\t{sqrt_val}")
```

**重要なポイント:**
- `math.sqrt(x)` は x の平方根を返す
- 結果は常に float 型
- 負の数に対してはエラーが発生する
- √x = x^(1/2) = x^0.5 の関係

**エラーハンドリングの例:**
```python
import math

def safe_sqrt(number):
    try:
        if number < 0:
            print(f"警告: {number}は負の数です。実数の平方根は存在しません。")
            return None
        else:
            result = math.sqrt(number)
            print(f"√{number} = {result}")
            return result
    except TypeError:
        print("エラー: 数値を入力してください。")
        return None

# テスト
safe_sqrt(81)   # 9.0
safe_sqrt(-4)   # 警告メッセージ
safe_sqrt(16)   # 4.0
```

<br>

---

<br>

問題 3
randomモジュールを利⽤して、1〜6のサイコロの出目をラン
ダムに出⼒するプログラムを作成してください。

**回答:**

**基本的なサイコロプログラム:**
```python
import random

# 1〜6のランダムな数値を生成
dice_result = random.randint(1, 6)
print(f"サイコロの出目: {dice_result}")
```

**実行結果例:**
```
サイコロの出目: 4
```

**詳細な実装例:**
```python
import random

def roll_dice():
    """1〜6のサイコロを振る関数"""
    return random.randint(1, 6)

def main():
    print("=== サイコロゲーム ===")
    
    # 1回サイコロを振る
    result = roll_dice()
    print(f"サイコロの出目: {result}")
    
    # 複数回振る例
    print("\n5回連続でサイコロを振ります:")
    for i in range(1, 6):
        dice = roll_dice()
        print(f"{i}回目: {dice}")

# プログラム実行
main()
```

**実行結果例:**
```
=== サイコロゲーム ===
サイコロの出目: 3

5回連続でサイコロを振ります:
1回目: 2
2回目: 6
3回目: 1
4回目: 4
5回目: 5
```

**応用版 - 視覚的なサイコロ:**
```python
import random

def visual_dice(number):
    """数字を視覚的なサイコロに変換"""
    dice_faces = {
        1: "⚀",
        2: "⚁", 
        3: "⚂",
        4: "⚃",
        5: "⚄",
        6: "⚅"
    }
    return dice_faces.get(number, "?")

def roll_visual_dice():
    """視覚的なサイコロを振る"""
    result = random.randint(1, 6)
    visual = visual_dice(result)
    print(f"サイコロの出目: {result} {visual}")
    return result

# 実行例
print("=== 視覚的サイコロ ===")
for i in range(3):
    roll_visual_dice()
```

**実行結果例:**
```
=== 視覚的サイコロ ===
サイコロの出目: 3 ⚂
サイコロの出目: 6 ⚅
サイコロの出目: 1 ⚀
```

**統計分析版:**
```python
import random
from collections import Counter

def dice_statistics(rolls=100):
    """指定回数サイコロを振って統計を取る"""
    results = []
    
    # 指定回数サイコロを振る
    for _ in range(rolls):
        results.append(random.randint(1, 6))
    
    # 統計を計算
    counter = Counter(results)
    
    print(f"=== {rolls}回のサイコロ統計 ===")
    for i in range(1, 7):
        count = counter[i]
        percentage = (count / rolls) * 100
        print(f"{i}: {count}回 ({percentage:.1f}%)")
    
    return results

# 統計実行
dice_statistics(60)
```

**randomモジュールの他の関数:**
```python
import random

# 異なるランダム関数の例
print("=== randomモジュールの例 ===")

# 1. randint(a, b) - a以上b以下の整数
print(f"randint(1, 6): {random.randint(1, 6)}")

# 2. choice(sequence) - リストから1つ選択
dice_faces = [1, 2, 3, 4, 5, 6]
print(f"choice([1,2,3,4,5,6]): {random.choice(dice_faces)}")

# 3. random() - 0.0以上1.0未満の浮動小数点数
random_float = random.random()
dice_from_float = int(random_float * 6) + 1
print(f"random()から作成: {dice_from_float}")
```

**重要なポイント:**
- `random.randint(1, 6)` で1〜6の整数をランダム生成
- 毎回実行するたびに異なる結果が出力される
- `random.seed(値)` で同じ結果を再現可能
- サイコロは各面が等確率(1/6)で出現する

<br>

---

<br>

問題 4
datetimeで現在の年だけを取得
現在の⻄暦年を画⾯上に表⽰してください。

**回答:**

**基本的な解答:**
```python
import datetime

# 現在の年を取得
current_year = datetime.datetime.now().year
print(f"現在の西暦年: {current_year}")
```

**実行結果:**
```
現在の西暦年: 2025
```

**詳細な実装例:**
```python
import datetime

# 方法1: datetime.datetime.now()を使用
now = datetime.datetime.now()
year1 = now.year
print(f"方法1 - 現在の年: {year1}")

# 方法2: datetime.date.today()を使用
today = datetime.date.today()
year2 = today.year
print(f"方法2 - 今日の年: {year2}")

# 方法3: 年だけを直接取得
year3 = datetime.date.today().year
print(f"方法3 - 年のみ: {year3}")

# 詳細な日時情報も表示
print(f"\n=== 詳細な日時情報 ===")
print(f"現在の日時: {now}")
print(f"年: {now.year}")
print(f"月: {now.month}")
print(f"日: {now.day}")
print(f"時: {now.hour}")
print(f"分: {now.minute}")
print(f"秒: {now.second}")
```

**実行結果:**
```
方法1 - 現在の年: 2025
方法2 - 今日の年: 2025
方法3 - 年のみ: 2025

=== 詳細な日時情報 ===
現在の日時: 2025-10-03 14:30:45.123456
年: 2025
月: 10
日: 3
時: 14
分: 30
秒: 45
```

**フォーマット付きの表示:**
```python
import datetime

def display_current_year():
    """現在の年を様々な形式で表示"""
    current_year = datetime.datetime.now().year
    
    print("=== 現在の年表示 ===")
    print(f"西暦: {current_year}年")
    print(f"Century: {current_year // 100 + 1}世紀")
    print(f"4桁表示: {current_year:04d}")
    print(f"令和: 令和{current_year - 2018}年")  # 令和は2019年開始

# 実行
display_current_year()
```

**実行結果:**
```
=== 現在の年表示 ===
西暦: 2025年
Century: 21世紀
4桁表示: 2025
令和: 令和7年
```

**年に関する計算例:**
```python
import datetime

def year_calculations():
    """年に関する様々な計算"""
    current_year = datetime.datetime.now().year
    
    print(f"現在の年: {current_year}")
    print(f"来年: {current_year + 1}")
    print(f"去年: {current_year - 1}")
    print(f"10年後: {current_year + 10}")
    print(f"100年前: {current_year - 100}")
    
    # うるう年判定
    is_leap = (current_year % 4 == 0 and current_year % 100 != 0) or (current_year % 400 == 0)
    print(f"{current_year}年はうるう年: {'はい' if is_leap else 'いいえ'}")

# 実行
year_calculations()
```

**datetime vs date の違い:**
```python
import datetime

print("=== datetime vs date の比較 ===")

# datetime.datetime - 日時（時刻込み）
dt = datetime.datetime.now()
print(f"datetime: {dt}")
print(f"datetime.year: {dt.year}")

# datetime.date - 日付のみ
d = datetime.date.today()
print(f"date: {d}")
print(f"date.year: {d.year}")

# 型の確認
print(f"datetime型: {type(dt)}")
print(f"date型: {type(d)}")
```

**重要なポイント:**
- `datetime.datetime.now().year` で現在の年を取得
- `datetime.date.today().year` でも同じ結果
- 結果は整数型（int）
- タイムゾーンを考慮する場合は`datetime.now(tz=...)`を使用
- 年だけでなく月、日、時間なども同様に取得可能

<br>

---

<br>

問題 5
calendarモジュールでカレンダーを表⽰
2025年８⽉の⽉間カレンダーを画⾯上に表⽰してください。

**回答:**

**基本的な解答:**
```python
import calendar

# 2025年8月のカレンダーを表示
calendar_output = calendar.month(2025, 8)
print(calendar_output)
```

**実行結果:**
```
    August 2025
Mo Tu We Th Fr Sa Su
             1  2  3
 4  5  6  7  8  9 10
11 12 13 14 15 16 17
18 19 20 21 22 23 24
25 26 27 28 29 30 31
```

**詳細な実装例:**
```python
import calendar

def display_calendar(year, month):
    """指定した年月のカレンダーを表示"""
    print(f"=== {year}年{month}月のカレンダー ===")
    cal = calendar.month(year, month)
    print(cal)

# 2025年8月のカレンダーを表示
display_calendar(2025, 8)

# 月名を日本語で表示
month_names_jp = {
    1: "一月", 2: "二月", 3: "三月", 4: "四月",
    5: "五月", 6: "六月", 7: "七月", 8: "八月", 
    9: "九月", 10: "十月", 11: "十一月", 12: "十二月"
}

print(f"\n{2025}年{month_names_jp[8]}:")
print(calendar.month(2025, 8))
```

**応用例 - 年間カレンダー:**
```python
import calendar

# 年間カレンダーの表示
print("=== 2025年の年間カレンダー ===")
year_calendar = calendar.calendar(2025)
print(year_calendar)

# 特定の月だけを表示
print("\n=== 2025年下半期のカレンダー ===")
for month in range(7, 13):  # 7月から12月
    month_name = calendar.month_name[month]
    print(f"\n{month_name} 2025:")
    print(calendar.month(2025, month))
```

**カレンダー情報の取得:**
```python
import calendar

def calendar_info(year, month):
    """カレンダーに関する詳細情報を表示"""
    print(f"=== {year}年{month}月の情報 ===")
    
    # 月のカレンダー表示
    print(calendar.month(year, month))
    
    # 月の日数
    days_in_month = calendar.monthrange(year, month)[1]
    print(f"この月の日数: {days_in_month}日")
    
    # 月の最初の日の曜日
    first_weekday = calendar.monthrange(year, month)[0]
    weekdays = ["月曜日", "火曜日", "水曜日", "木曜日", "金曜日", "土曜日", "日曜日"]
    print(f"月初の曜日: {weekdays[first_weekday]}")
    
    # うるう年判定
    is_leap = calendar.isleap(year)
    print(f"{year}年はうるう年: {'はい' if is_leap else 'いいえ'}")

# 2025年8月の詳細情報
calendar_info(2025, 8)
```

**実行結果:**
```
=== 2025年8月の情報 ===
    August 2025
Mo Tu We Th Fr Sa Su
             1  2  3
 4  5  6  7  8  9 10
11 12 13 14 15 16 17
18 19 20 21 22 23 24
25 26 27 28 29 30 31

この月の日数: 31日
月初の曜日: 金曜日
2025年はうるう年: いいえ
```

**calendarモジュールの主要関数:**
```python
import calendar

print("=== calendarモジュールの機能 ===")

# 1. month(year, month) - 月のカレンダー
print("1. 月のカレンダー:")
print(calendar.month(2025, 8))

# 2. monthrange(year, month) - 月の情報
print("2. 月の範囲情報:")
print(f"monthrange(2025, 8): {calendar.monthrange(2025, 8)}")

# 3. weekday(year, month, day) - 曜日取得
print("3. 曜日取得:")
print(f"2025年8月1日の曜日: {calendar.weekday(2025, 8, 1)}")  # 0=月曜日

# 4. isleap(year) - うるう年判定
print("4. うるう年判定:")
print(f"2025年: {calendar.isleap(2025)}")
print(f"2024年: {calendar.isleap(2024)}")
```

**重要なポイント:**
- `calendar.month(year, month)` で指定月のカレンダーを取得
- 曜日は月曜日から始まる（Mon=0, Sun=6）
- `calendar.monthrange()` で月の日数と開始曜日を取得
- 英語表示だが、日本語ラベルを追加可能
- カレンダーは文字列として返される

<br>

---

<br>

問題 6
sysモジュールでpythonバージョンを表⽰
現在のPythonバージョンを画⾯上に表⽰してください。

**回答:**

**基本的な解答:**
```python
import sys

# Pythonバージョンを表示
print(f"Pythonバージョン: {sys.version}")
```

**実行結果例:**
```
Pythonバージョン: 3.11.5 (main, Aug 24 2023, 15:18:16) [MSC v.1916 64 bit (AMD64)]
```

**詳細な実装例:**
```python
import sys

def display_python_info():
    """Python環境の詳細情報を表示"""
    print("=== Python環境情報 ===")
    
    # 1. 基本バージョン情報
    print(f"Pythonバージョン: {sys.version}")
    print(f"バージョン情報: {sys.version_info}")
    
    # 2. 簡潔なバージョン表示
    version_short = f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
    print(f"簡潔版: Python {version_short}")
    
    # 3. プラットフォーム情報
    print(f"プラットフォーム: {sys.platform}")
    
    # 4. 実行ファイルのパス
    print(f"Python実行ファイル: {sys.executable}")
    
    # 5. モジュール検索パス
    print(f"モジュール検索パス数: {len(sys.path)}個")

# 実行
display_python_info()
```

**実行結果例:**
```
=== Python環境情報 ===
Pythonバージョン: 3.11.5 (main, Aug 24 2023, 15:18:16) [MSC v.1916 64 bit (AMD64)]
バージョン情報: sys.version_info(major=3, minor=11, micro=5, releaselevel='final', serial=0)
簡潔版: Python 3.11.5
プラットフォーム: win32
Python実行ファイル: C:\Python311\python.exe
モジュール検索パス数: 8個
```

**異なるバージョン表示方法:**
```python
import sys

def version_display_options():
    """様々なバージョン表示方法"""
    print("=== 様々なバージョン表示 ===")
    
    # 方法1: sys.version（完全な情報）
    print(f"1. 完全版: {sys.version}")
    
    # 方法2: sys.version_info（構造化された情報）
    print(f"2. 構造化: {sys.version_info}")
    
    # 方法3: メジャー.マイナー.マイクロ
    v = sys.version_info
    print(f"3. 標準形式: {v.major}.{v.minor}.{v.micro}")
    
    # 方法4: メジャー.マイナーのみ
    print(f"4. 簡易形式: {v.major}.{v.minor}")
    
    # 方法5: 条件分岐での使用例
    if v.major >= 3 and v.minor >= 8:
        print("5. Python 3.8以上です")
    else:
        print("5. Python 3.8未満です")

version_display_options()
```

**バージョン比較の例:**
```python
import sys

def version_check():
    """Pythonバージョンのチェックと比較"""
    version = sys.version_info
    
    print(f"現在のPython: {version.major}.{version.minor}.{version.micro}")
    
    # 特定バージョンとの比較
    if version >= (3, 8):
        print("✓ Python 3.8以上 - 代入式(:=)が使用可能")
    
    if version >= (3, 9):
        print("✓ Python 3.9以上 - 辞書結合演算子(|)が使用可能")
    
    if version >= (3, 10):
        print("✓ Python 3.10以上 - match文が使用可能")
    
    if version >= (3, 11):
        print("✓ Python 3.11以上 - 高速化とエラーメッセージ改善")
    
    # EOL（サポート終了）チェック
    if version.major == 2:
        print("⚠️ Python 2はサポート終了済みです")
    elif version < (3, 7):
        print("⚠️ 古いバージョンです。アップデートを推奨します")

version_check()
```

**システム情報も含めた総合表示:**
```python
import sys
import platform

def comprehensive_system_info():
    """システムとPythonの総合情報"""
    print("=== システム・Python総合情報 ===")
    
    # Python情報
    print(f"Python: {sys.version.split()[0]}")
    print(f"バージョン: {sys.version_info}")
    print(f"実行ファイル: {sys.executable}")
    
    # システム情報（platformモジュール併用）
    print(f"OS: {platform.system()} {platform.release()}")
    print(f"アーキテクチャ: {platform.architecture()[0]}")
    print(f"プロセッサ: {platform.processor()}")
    print(f"マシン: {platform.machine()}")
    
    # エンコーディング情報
    print(f"デフォルトエンコーディング: {sys.getdefaultencoding()}")
    print(f"ファイルシステムエンコーディング: {sys.getfilesystemencoding()}")

comprehensive_system_info()
```

**sysモジュールの他の便利な機能:**
```python
import sys

print("=== sysモジュールの機能 ===")

# 1. コマンドライン引数
print(f"スクリプト名: {sys.argv[0]}")
print(f"引数の数: {len(sys.argv)}")

# 2. モジュール検索パス
print(f"モジュールパス数: {len(sys.path)}")

# 3. 最大再帰深度
print(f"最大再帰深度: {sys.getrecursionlimit()}")

# 4. インポート済みモジュール数
print(f"インポート済みモジュール数: {len(sys.modules)}")

# 5. Pythonの整数の最大値（Python 3では実質無制限）
print(f"最大整数サイズ情報: {sys.maxsize}")
```

**重要なポイント:**
- `sys.version` で完全なバージョン情報を取得
- `sys.version_info` で構造化されたバージョン情報
- バージョン比較は `sys.version_info >= (3, 8)` の形式で可能
- プラットフォーム固有の情報も `sys.platform` で取得可能
- スクリプトの実行環境を調べるのに便利

<br>

---

<br>

問題 7
randomで乱数をリストから選ぶ問題
[“グー”, “チョキ”, “パー”] からランダムに1つ選んで画⾯上に
表⽰してください。

**回答:**

**基本的な解答:**
```python
import random

# じゃんけんの選択肢
choices = ["グー", "チョキ", "パー"]

# ランダムに1つ選択
result = random.choice(choices)
print(f"選択された手: {result}")
```

**実行結果例:**
```
選択された手: パー
```

**詳細な実装例:**
```python
import random

def janken_choice():
    """じゃんけんの手をランダムに選択"""
    choices = ["グー", "チョキ", "パー"]
    selected = random.choice(choices)
    
    print(f"=== じゃんけん ===")
    print(f"コンピュータの手: {selected}")
    
    return selected

# 実行
janken_choice()
```

**応用例 - じゃんけんゲーム:**
```python
import random

def janken_game():
    """完全なじゃんけんゲーム"""
    choices = ["グー", "チョキ", "パー"]
    
    print("=== じゃんけんゲーム ===")
    print("選択肢: 1.グー 2.チョキ 3.パー")
    
    # プレイヤーの入力（実際の実装では input() を使用）
    player_choice = "グー"  # 例として固定
    computer_choice = random.choice(choices)
    
    print(f"あなたの手: {player_choice}")
    print(f"コンピュータの手: {computer_choice}")
    
    # 勝敗判定
    if player_choice == computer_choice:
        result = "引き分け"
    elif (player_choice == "グー" and computer_choice == "チョキ") or \
         (player_choice == "チョキ" and computer_choice == "パー") or \
         (player_choice == "パー" and computer_choice == "グー"):
        result = "あなたの勝ち"
    else:
        result = "コンピュータの勝ち"
    
    print(f"結果: {result}")

janken_game()
```

**複数回選択の例:**
```python
import random

def multiple_choices():
    """複数回選択して統計を取る"""
    choices = ["グー", "チョキ", "パー"]
    results = []
    
    print("=== 10回連続選択 ===")
    for i in range(10):
        selected = random.choice(choices)
        results.append(selected)
        print(f"{i+1}回目: {selected}")
    
    # 統計
    print(f"\n=== 統計 ===")
    for choice in choices:
        count = results.count(choice)
        print(f"{choice}: {count}回")

multiple_choices()
```

**他のリストでの応用例:**
```python
import random

def various_random_choices():
    """様々なリストからのランダム選択例"""
    
    # 1. 色の選択
    colors = ["赤", "青", "緑", "黄", "紫"]
    selected_color = random.choice(colors)
    print(f"選択された色: {selected_color}")
    
    # 2. 食べ物の選択
    foods = ["寿司", "ラーメン", "カレー", "パスタ", "ハンバーガー"]
    selected_food = random.choice(foods)
    print(f"今日の昼食: {selected_food}")
    
    # 3. 数字の選択
    numbers = [10, 20, 30, 40, 50]
    selected_number = random.choice(numbers)
    print(f"選択された数字: {selected_number}")

various_random_choices()
```

**重要なポイント:**
- `random.choice(sequence)` でシーケンスからランダムに1つ選択
- リスト、タプル、文字列など任意のシーケンスに使用可能
- 空のシーケンスに対してはIndexErrorが発生
- `random.choices()` で重み付き選択や複数選択も可能
- 毎回実行するたびに異なる結果が得られる

<br>

---

<br>

問題 8
randomでリストをシャッフル
リスト[1,2,3,4,5]をランダムな順番に並び替えて、画⾯上に表
⽰してください。

**回答:**

**基本的な解答:**
```python
import random

# 元のリスト
numbers = [1, 2, 3, 4, 5]
print(f"元のリスト: {numbers}")

# リストをシャッフル（元のリストを変更）
random.shuffle(numbers)
print(f"シャッフル後: {numbers}")
```

**実行結果例:**
```
元のリスト: [1, 2, 3, 4, 5]
シャッフル後: [3, 1, 5, 2, 4]
```

**詳細な実装例:**
```python
import random

def shuffle_list(original_list):
    """リストをシャッフルする関数"""
    # 元のリストのコピーを作成（元のリストを保持）
    shuffled_list = original_list.copy()
    random.shuffle(shuffled_list)
    
    print(f"元のリスト: {original_list}")
    print(f"シャッフル後: {shuffled_list}")
    
    return shuffled_list

# 実行
test_list = [1, 2, 3, 4, 5]
result = shuffle_list(test_list)
```

**複数回シャッフルの例:**
```python
import random

def multiple_shuffles(original_list, count=5):
    """複数回シャッフルして結果を表示"""
    print(f"元のリスト: {original_list}")
    print("=" * 30)
    
    for i in range(count):
        shuffled = original_list.copy()
        random.shuffle(shuffled)
        print(f"{i+1}回目: {shuffled}")

# 実行
numbers = [1, 2, 3, 4, 5]
multiple_shuffles(numbers)
```

**実行結果例:**
```
元のリスト: [1, 2, 3, 4, 5]
==============================
1回目: [4, 1, 3, 5, 2]
2回目: [2, 5, 1, 3, 4]
3回目: [3, 4, 2, 1, 5]
4回目: [5, 2, 4, 1, 3]
5回目: [1, 3, 5, 4, 2]
```

**異なる種類のリストのシャッフル:**
```python
import random

def shuffle_various_lists():
    """様々な種類のリストをシャッフル"""
    
    # 1. 数字のリスト
    numbers = [1, 2, 3, 4, 5]
    shuffled_numbers = numbers.copy()
    random.shuffle(shuffled_numbers)
    print(f"数字: {numbers} → {shuffled_numbers}")
    
    # 2. 文字のリスト
    letters = ['A', 'B', 'C', 'D', 'E']
    shuffled_letters = letters.copy()
    random.shuffle(shuffled_letters)
    print(f"文字: {letters} → {shuffled_letters}")
    
    # 3. 文字列のリスト
    words = ["apple", "banana", "cherry", "date"]
    shuffled_words = words.copy()
    random.shuffle(shuffled_words)
    print(f"単語: {words} → {shuffled_words}")
    
    # 4. 混合型のリスト
    mixed = [1, "hello", 3.14, True]
    shuffled_mixed = mixed.copy()
    random.shuffle(shuffled_mixed)
    print(f"混合: {mixed} → {shuffled_mixed}")

shuffle_various_lists()
```

**カードデッキのシャッフル例:**
```python
import random

def create_and_shuffle_deck():
    """トランプのデッキを作成してシャッフル"""
    # スートと数字
    suits = ["♠", "♥", "♦", "♣"]
    values = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"]
    
    # デッキを作成
    deck = []
    for suit in suits:
        for value in values:
            deck.append(f"{value}{suit}")
    
    print("=== トランプデッキ ===")
    print(f"作成されたデッキ（最初の10枚）: {deck[:10]}")
    print(f"デッキの総数: {len(deck)}枚")
    
    # シャッフル
    random.shuffle(deck)
    print(f"シャッフル後（最初の10枚）: {deck[:10]}")
    
    # 5枚配る
    hand = deck[:5]
    print(f"配られた手札: {hand}")

create_and_shuffle_deck()
```

**shuffle()とsample()の比較:**
```python
import random

def compare_shuffle_methods():
    """shuffle()とsample()の比較"""
    original = [1, 2, 3, 4, 5]
    
    print(f"元のリスト: {original}")
    print("=" * 30)
    
    # 方法1: random.shuffle()（元のリストを変更）
    list1 = original.copy()
    random.shuffle(list1)
    print(f"shuffle()使用: {list1}")
    
    # 方法2: random.sample()（新しいリストを作成）
    list2 = random.sample(original, len(original))
    print(f"sample()使用: {list2}")
    
    # 方法3: sorted()とrandom.random()
    list3 = sorted(original, key=lambda x: random.random())
    print(f"sorted()使用: {list3}")
    
    print(f"元のリスト確認: {original}")  # 変更されていない

compare_shuffle_methods()
```

**シャッフルアルゴリズムの実装例:**
```python
import random

def manual_shuffle(lst):
    """手動でのシャッフル実装（Fisher-Yates法）"""
    result = lst.copy()
    
    for i in range(len(result) - 1, 0, -1):
        # 0からiまでのランダムなインデックス
        j = random.randint(0, i)
        # 要素を交換
        result[i], result[j] = result[j], result[i]
    
    return result

def compare_shuffle_algorithms():
    """組み込みシャッフルと手動実装の比較"""
    original = [1, 2, 3, 4, 5]
    
    # 組み込みshuffle()
    list1 = original.copy()
    random.shuffle(list1)
    
    # 手動実装
    list2 = manual_shuffle(original)
    
    print(f"元のリスト: {original}")
    print(f"random.shuffle(): {list1}")
    print(f"手動実装: {list2}")

compare_shuffle_algorithms()
```

**ゲーム用途の例:**
```python
import random

def rock_paper_scissors_shuffle():
    """じゃんけんのランダム戦略"""
    strategies = ["グー", "チョキ", "パー"]
    
    # 10回分の戦略をランダムに決める
    game_plan = strategies * 4  # [グー, チョキ, パー] × 4 = 12個
    random.shuffle(game_plan)
    
    print("=== じゃんけん戦略（10回分） ===")
    for i in range(10):
        print(f"{i+1}回目: {game_plan[i]}")

def quiz_question_shuffle():
    """クイズ問題のシャッフル"""
    questions = [
        "Pythonの開発者は？",
        "Pythonの名前の由来は？", 
        "Pythonのインデントは何文字？",
        "Pythonの拡張子は？",
        "Pythonのバージョン3はいつリリース？"
    ]
    
    print("=== クイズ問題 ===")
    print("元の順番:")
    for i, q in enumerate(questions, 1):
        print(f"{i}. {q}")
    
    # シャッフル
    shuffled_questions = questions.copy()
    random.shuffle(shuffled_questions)
    
    print("\nシャッフル後:")
    for i, q in enumerate(shuffled_questions, 1):
        print(f"{i}. {q}")

# 実行
rock_paper_scissors_shuffle()
print("=" * 40)
quiz_question_shuffle()
```

**重要なポイント:**
- `random.shuffle(list)` でリストを**その場で**シャッフル（元のリストが変更される）
- 元のリストを保持したい場合は事前に `list.copy()` でコピーを作成
- `random.sample(list, len(list))` で新しいシャッフル済みリストを作成
- シャッフルは毎回異なる結果になる
- リストの順序をランダム化するのに便利（ゲーム、クイズ、テストデータなど）

<br>

---

<br>

問題 9
整数リスト [1,2,3] の合計値を算出し、画⾯上に表⽰してくだ
さい。

**回答:**

**基本的な解答:**
```python
# リストの合計値を取得
numbers = [1, 2, 3]
total = sum(numbers)
print(f"リスト {numbers} の合計値: {total}")
```

**実行結果:**
```
リスト [1, 2, 3] の合計値: 6
```

**詳細な実装例:**
```python
def calculate_sum(numbers):
    """リストの合計値を計算する関数"""
    if not numbers:
        print("エラー: 空のリストです")
        return 0
    
    total = sum(numbers)
    print(f"リスト {numbers} の合計値: {total}")
    return total

# 実行例
test_list = [1, 2, 3]
result = calculate_sum(test_list)
```

**様々なリストでの例:**
```python
# 異なるリストの合計値
lists = [
    [1, 2, 3],
    [5, 10, 2, 8],
    [-1, -5, 3],
    [3.14, 2.71, 1.41],
    [100, 50, 75, 25]
]

print("=== 様々なリストの合計値 ===")
for i, lst in enumerate(lists, 1):
    total = sum(lst)
    print(f"{i}. {lst} → 合計値: {total}")
```

**実行結果:**
```
=== 様々なリストの合計値 ===
1. [1, 2, 3] → 合計値: 6
2. [5, 10, 2, 8] → 合計値: 25
3. [-1, -5, 3] → 合計値: -3
4. [3.14, 2.71, 1.41] → 合計値: 7.26
5. [100, 50, 75, 25] → 合計値: 250
```

**sum()関数の様々な使用方法:**
```python
# 1. 基本的な使用
numbers = [1, 2, 3]
print(f"合計値: {sum(numbers)}")

# 2. 初期値を指定
print(f"初期値10を加えた合計: {sum(numbers, 10)}")

# 3. 範囲の合計
print(f"1から10の合計: {sum(range(1, 11))}")

# 4. 条件付き合計（偶数のみ）
even_sum = sum(x for x in numbers if x % 2 == 0)
print(f"偶数の合計: {even_sum}")

# 5. 2次元リストの各行の合計
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
for i, row in enumerate(matrix):
    row_sum = sum(row)
    print(f"行{i+1}の合計: {row_sum}")
```

**実行結果:**
```
合計値: 6
初期値10を加えた合計: 16
1から10の合計: 55
偶数の合計: 2
行1の合計: 6
行2の合計: 15
行3の合計: 24
```

**手動での合計計算との比較:**
```python
def manual_sum(numbers):
    """forループを使った手動合計計算"""
    total = 0
    for num in numbers:
        total += num
    return total

def compare_sum_methods(numbers):
    """sum()関数と手動計算の比較"""
    # sum()関数を使用
    builtin_sum = sum(numbers)
    
    # 手動計算
    manual_result = manual_sum(numbers)
    
    print(f"リスト: {numbers}")
    print(f"sum()関数: {builtin_sum}")
    print(f"手動計算: {manual_result}")
    print(f"結果が同じ: {builtin_sum == manual_result}")

# 実行
test_lists = [
    [1, 2, 3],
    [10, 20, 30, 40],
    [-5, 5, -3, 3]
]

for lst in test_lists:
    compare_sum_methods(lst)
    print("---")
```

**統計情報と組み合わせた例:**
```python
def list_statistics(numbers):
    """リストの統計情報を表示"""
    if not numbers:
        print("空のリストです")
        return
    
    total = sum(numbers)
    count = len(numbers)
    average = total / count
    maximum = max(numbers)
    minimum = min(numbers)
    
    print(f"リスト: {numbers}")
    print(f"合計値: {total}")
    print(f"要素数: {count}")
    print(f"平均値: {average:.2f}")
    print(f"最大値: {maximum}")
    print(f"最小値: {minimum}")

# 実行
test_lists = [
    [1, 2, 3],
    [10, 5, 15, 20, 8],
    [2, 4, 6, 8, 10]
]

for lst in test_lists:
    list_statistics(lst)
    print("=" * 25)
```

**実行結果:**
```
リスト: [1, 2, 3]
合計値: 6
要素数: 3
平均値: 2.00
最大値: 3
最小値: 1
=========================
リスト: [10, 5, 15, 20, 8]
合計値: 58
要素数: 5
平均値: 11.60
最大値: 20
最小値: 5
=========================
```

**エラーハンドリング付きの例:**
```python
def safe_sum(numbers):
    """安全な合計計算（エラーハンドリング付き）"""
    try:
        if not isinstance(numbers, list):
            print("エラー: リストを入力してください")
            return None
        
        if not numbers:
            print("警告: 空のリストです。合計値は0です")
            return 0
        
        # 数値以外の要素をチェック
        if not all(isinstance(x, (int, float)) for x in numbers):
            print("警告: 数値以外の要素が含まれています")
            numbers = [x for x in numbers if isinstance(x, (int, float))]
            if not numbers:
                print("エラー: 数値が見つかりません")
                return None
        
        total = sum(numbers)
        print(f"合計値: {total}")
        return total
        
    except Exception as e:
        print(f"エラーが発生しました: {e}")
        return None

# テスト
safe_sum([1, 2, 3])      # 正常
safe_sum([])             # 空リスト
safe_sum([1, "a", 3])    # 混在型
safe_sum("123")          # 不正な型
```

**重要なポイント:**
- `sum(list)` でリストの合計値を取得
- 初期値を指定できる: `sum(list, start_value)`
- 空のリストの場合は0を返す
- 数値以外の要素があるとTypeErrorが発生
- ジェネレータ式と組み合わせて条件付き合計も可能

<br>

---

<br>

問題 10
リスト [1,2,3] の最大値を算出し、画⾯上に表⽰してください。

**回答:**

**基本的な解答:**
```python
# リストの最大値を取得
numbers = [1, 2, 3]
maximum = max(numbers)
print(f"リスト {numbers} の最大値: {maximum}")
```

**実行結果:**
```
リスト [1, 2, 3] の最大値: 3
```

**詳細な実装例:**
```python
def find_maximum(numbers):
    """リストの最大値を見つける関数"""
    if not numbers:
        print("エラー: 空のリストです")
        return None
    
    maximum = max(numbers)
    print(f"リスト {numbers} の最大値: {maximum}")
    return maximum

# 実行例
test_list = [1, 2, 3]
result = find_maximum(test_list)
```

**様々なリストでの例:**
```python
# 異なるリストの最大値
lists = [
    [1, 2, 3],
    [5, 10, 2, 8],
    [-1, -5, -3],
    [3.14, 2.71, 1.41],
    [100, 50, 75, 25]
]

print("=== 様々なリストの最大値 ===")
for i, lst in enumerate(lists, 1):
    maximum = max(lst)
    print(f"{i}. {lst} → 最大値: {maximum}")
```

**実行結果:**
```
=== 様々なリストの最大値 ===
1. [1, 2, 3] → 最大値: 3
2. [5, 10, 2, 8] → 最大値: 10
3. [-1, -5, -3] → 最大値: -1
4. [3.14, 2.71, 1.41] → 最大値: 3.14
5. [100, 50, 75, 25] → 最大値: 100
```

**max()関数の様々な使用方法:**
```python
# 1. 基本的な使用
numbers = [1, 2, 3]
print(f"最大値: {max(numbers)}")

# 2. 複数の引数として渡す
print(f"最大値: {max(1, 2, 3)}")

# 3. 文字列のリスト（辞書順）
words = ["apple", "banana", "cherry"]
print(f"辞書順最大: {max(words)}")

# 4. key関数を使用（文字列の長さで比較）
longest = max(words, key=len)
print(f"最長文字列: {longest}")

# 5. 2次元リストの各行の最大値
matrix = [[1, 2, 3], [4, 9, 6], [7, 8, 2]]
for i, row in enumerate(matrix):
    print(f"行{i+1}の最大値: {max(row)}")
```

**実行結果:**
```
最大値: 3
最大値: 3
辞書順最大: cherry
最長文字列: banana
行1の最大値: 3
行2の最大値: 9
行3の最大値: 8
```

**最大値の位置（インデックス）も取得:**
```python
def max_with_index(numbers):
    """最大値とその位置を取得"""
    if not numbers:
        return None, None
    
    maximum = max(numbers)
    index = numbers.index(maximum)
    
    print(f"リスト: {numbers}")
    print(f"最大値: {maximum}")
    print(f"位置: インデックス {index}")
    
    return maximum, index

# 実行
test_lists = [
    [1, 2, 3],
    [5, 2, 8, 1, 7],
    [3, 3, 9, 3]
]

for lst in test_lists:
    max_val, max_idx = max_with_index(lst)
    print("---")
```

**min()との比較:**
```python
def analyze_list(numbers):
    """リストの最大値・最小値・範囲を分析"""
    if not numbers:
        print("空のリストです")
        return
    
    maximum = max(numbers)
    minimum = min(numbers)
    range_val = maximum - minimum
    
    print(f"リスト: {numbers}")
    print(f"最大値: {maximum}")
    print(f"最小値: {minimum}")
    print(f"範囲: {range_val}")
    print(f"平均値: {sum(numbers) / len(numbers):.2f}")

# 実行
test_lists = [
    [1, 2, 3],
    [10, 5, 15, 3, 12],
    [-2, 0, 2, -1]
]

for lst in test_lists:
    analyze_list(lst)
    print("=" * 20)
```

**重要なポイント:**
- `max(list)` でリストの最大値を取得
- 空のリストに対してはValueErrorが発生
- 数値だけでなく文字列や他の比較可能なオブジェクトにも使用可能
- `key` パラメータで比較基準をカスタマイズ可能
- `min()` と組み合わせてデータの範囲を分析可能

<br>

---

<br>

問題 11
リスト [1,2,3] の最小値を算出し、画⾯上に表⽰してください。

**回答:**

**基本的な解答:**
```python
# リストの最小値を取得
numbers = [1, 2, 3]
minimum = min(numbers)
print(f"リスト {numbers} の最小値: {minimum}")
```

**実行結果:**
```
リスト [1, 2, 3] の最小値: 1
```

**詳細な実装例:**
```python
def find_minimum(numbers):
    """リストの最小値を見つける関数"""
    if not numbers:
        print("エラー: 空のリストです")
        return None
    
    minimum = min(numbers)
    print(f"リスト {numbers} の最小値: {minimum}")
    return minimum

# 実行例
test_list = [1, 2, 3]
result = find_minimum(test_list)
```

**様々なリストでの例:**
```python
# 異なるリストの最小値
lists = [
    [1, 2, 3],
    [5, 10, 2, 8],
    [-1, -5, -3],
    [3.14, 2.71, 1.41],
    [100, 50, 75, 25]
]

print("=== 様々なリストの最小値 ===")
for i, lst in enumerate(lists, 1):
    minimum = min(lst)
    print(f"{i}. {lst} → 最小値: {minimum}")
```

**実行結果:**
```
=== 様々なリストの最小値 ===
1. [1, 2, 3] → 最小値: 1
2. [5, 10, 2, 8] → 最小値: 2
3. [-1, -5, -3] → 最小値: -5
4. [3.14, 2.71, 1.41] → 最小値: 1.41
5. [100, 50, 75, 25] → 最小値: 25
```

**min()関数の様々な使用方法:**
```python
# 1. 基本的な使用
numbers = [1, 2, 3]
print(f"最小値: {min(numbers)}")

# 2. 複数の引数として渡す
print(f"最小値: {min(1, 2, 3)}")

# 3. 文字列のリスト（辞書順）
words = ["apple", "banana", "cherry"]
print(f"辞書順最小: {min(words)}")

# 4. key関数を使用（文字列の長さで比較）
shortest = min(words, key=len)
print(f"最短文字列: {shortest}")

# 5. 2次元リストの各行の最小値
matrix = [[1, 2, 3], [4, 0, 6], [7, 8, 2]]
for i, row in enumerate(matrix):
    print(f"行{i+1}の最小値: {min(row)}")
```

**実行結果:**
```
最小値: 1
最小値: 1
辞書順最小: apple
最短文字列: apple
行1の最小値: 1
行2の最小値: 0
行3の最小値: 2
```

**エラーハンドリング付きの例:**
```python
def safe_min(numbers):
    """安全な最小値取得（エラーハンドリング付き）"""
    try:
        if not numbers:
            print("警告: 空のリストです")
            return None
        
        if not all(isinstance(x, (int, float)) for x in numbers):
            print("警告: 数値以外の要素が含まれています")
            # 数値のみを抽出
            numbers = [x for x in numbers if isinstance(x, (int, float))]
            if not numbers:
                print("エラー: 数値が見つかりません")
                return None
        
        minimum = min(numbers)
        print(f"最小値: {minimum}")
        return minimum
        
    except Exception as e:
        print(f"エラーが発生しました: {e}")
        return None

# テスト
safe_min([1, 2, 3])        # 正常
safe_min([])               # 空リスト
safe_min([1, "a", 3])      # 混在型
safe_min(["a", "b"])       # 非数値
```

**実行結果:**
```
最小値: 1
警告: 空のリストです
警告: 数値以外の要素が含まれています
最小値: 1
警告: 数値以外の要素が含まれています
エラー: 数値が見つかりません
```

**最小値の位置（インデックス）も取得:**
```python
def min_with_index(numbers):
    """最小値とその位置を取得"""
    if not numbers:
        return None, None
    
    minimum = min(numbers)
    index = numbers.index(minimum)
    
    print(f"リスト: {numbers}")
    print(f"最小値: {minimum}")
    print(f"位置: インデックス {index}")
    
    return minimum, index

# 実行
test_lists = [
    [1, 2, 3],
    [5, 2, 8, 1, 7],
    [3, 3, 1, 3]
]

for lst in test_lists:
    min_val, min_idx = min_with_index(lst)
    print("---")
```

**重要なポイント:**
- `min(list)` でリストの最小値を取得
- 空のリストに対してはValueErrorが発生
- 数値だけでなく文字列や他の比較可能なオブジェクトにも使用可能
- `key` パラメータで比較基準をカスタマイズ可能
- 複数の値が同じ最小値の場合、最初に見つかった値を返す

<br>

---

<br>
