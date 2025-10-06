# コレクション問題解答集

## 問題 1
次の説明⽂が、リスト、タプル、辞書、セットのいずれに該当するか、答えてください

**解答:**
- （1）キーと値のペアを格納する → **辞書（dict）**
- （2）要素の値の重複が許されない → **セット（set）**
- （3）要素の値を変更できない → **タプル（tuple）**
- （4）インデックスで要素にアクセスできる → **リスト（list）、タプル（tuple）**

**解説:**
- **辞書（dict）**: `{"key": "value"}` の形式でキーと値のペアを格納します。キーを使って効率的に値にアクセスできます。
- **セット（set）**: `{1, 2, 3}` の形式で要素を格納し、重複を自動的に排除します。数学の集合演算も可能です。
- **タプル（tuple）**: `(1, 2, 3)` の形式で要素を格納し、作成後は変更できません（不変オブジェクト）。
- **リスト（list）**: `[1, 2, 3]` の形式で要素を格納し、インデックスでアクセス可能。要素の変更も可能です。

## 問題 2
nums = [10,20,30,40] の2番目の要素（20）を99に変更

**解答:**
```python
nums = [10, 20, 30, 40]
nums[1] = 99
print(nums)
```

**実行結果:**
```
[10, 99, 30, 40]
```

**解説:**
- リストのインデックスは0から始まります（0ベースインデックス）
- 2番目の要素は `nums[1]` でアクセスします
- `nums[1] = 99` で直接値を変更できます（リストは可変オブジェクト）
- 変更後は元のリストが更新されます

## 問題 3
fruits = ['apple','banana'] に'grape'を末尾に追加

**解答:**
```python
fruits = ['apple', 'banana']
fruits.append('grape')
print(fruits)
```

**実行結果:**
```
['apple', 'banana', 'grape']
```

**解説:**
- `append()` メソッドはリストの末尾に要素を1つ追加します
- 元のリストが直接変更されます（インプレース操作）
- 戻り値は `None` です（新しいリストは作成されません）
- 他の追加方法: `insert(位置, 要素)` で任意の位置に挿入可能

## 問題 4
fruits = ['apple','banana','grape'] から'banana'を削除

**解答:**
```python
fruits = ['apple', 'banana', 'grape']
fruits.remove('banana')
print(fruits)  # ['apple', 'grape']
```

**解説:**
- `remove()` メソッドは指定した値と一致する最初の要素を削除します
- 要素が存在しない場合は `ValueError` が発生します
- 他の削除方法:
  - `pop(インデックス)`: 指定位置の要素を削除して返す
  - `del fruits[インデックス]`: 指定位置の要素を削除
  - `clear()`: すべての要素を削除

## 問題 5
nums = [10,20,30,40,50] から「20,30」を取り出し（スライス）

**解答:**
```python
nums = [10, 20, 30, 40, 50]
result = nums[1:3]  # インデックス1から2まで
print(result)  # [20, 30]
```

**解説:**
- スライス記法: `リスト[開始:終了]`
- 開始インデックスは含まれ、終了インデックスは含まれません
- `nums[1:3]` はインデックス1と2の要素を取得
- 新しいリストが作成されます（元のリストは変更されません）
- 省略形: `nums[:3]`（先頭から）、`nums[1:]`（末尾まで）

## 問題 6
data = [1,2,3,4] の先頭2つを[100,200]に変更（スライス）

**解答:**
```python
data = [1, 2, 3, 4]
data[0:2] = [100, 200]
print(data)  # [100, 200, 3, 4]
```

**解説:**
- スライス代入を使用してリストの一部を置き換えます
- `data[0:2] = [100, 200]` はインデックス0と1の要素を新しい値で置換
- 置換する要素数と新しい要素数は異なっても構いません
- 例: `data[0:2] = [100, 200, 300]` とすると3つの要素で置換される

## 問題 7
fruits = ['apple','banana'] の先頭に'lemon'を追加

**解答:**
```python
fruits = ['apple', 'banana']
fruits.insert(0, 'lemon')  # インデックス0に挿入
print(fruits)  # ['lemon', 'apple', 'banana']
```

**解説:**
- `insert(位置, 要素)` メソッドで指定した位置に要素を挿入します
- インデックス0に挿入すると先頭に追加されます
- 既存の要素は右にシフトされます
- `append()` との違い: `append()` は常に末尾、`insert()` は任意の位置

## 問題 8
items = [1,2,3,4] の末尾の要素を削除

**解答:**
```python
items = [1, 2, 3, 4]
items.pop()  # 末尾を削除
print(items)  # [1, 2, 3]
```

**解説:**
- `pop()` メソッドは末尾の要素を削除して、その要素を返します
- `pop(インデックス)` で任意の位置の要素を削除可能
- 削除された要素を変数に保存可能: `removed_item = items.pop()`
- リストが空の場合は `IndexError` が発生

## 問題 9
名前と年齢のディクショナリを作成

**解答:**
```python
person = {'name': 'Taro', 'age': '20'}
print(person)  # {'name': 'Taro', 'age': '20'}
```

**解説:**
- 辞書は `{キー: 値}` の形式で作成します
- キーは文字列、数値、タプルなど不変オブジェクトが使用可能
- 値は任意のオブジェクトを格納できます
- 他の作成方法: `dict(name='Taro', age='20')` や `dict([('name', 'Taro'), ('age', '20')])`

## 問題 10
profile = {'name': 'Hanako', 'age': 25, 'city': 'Tokyo'} から'city'の値を取得

**解答:**
```python
profile = {'name': 'Hanako', 'age': 25, 'city': 'Tokyo'}
print(profile['city'])  # Tokyo
```

**解説:**
- 辞書の値は `辞書[キー]` でアクセスします
- キーが存在しない場合は `KeyError` が発生します
- 安全なアクセス方法: `profile.get('city')` - キーがない場合は `None` を返す
- デフォルト値指定: `profile.get('country', 'Japan')` - キーがない場合は 'Japan' を返す

## 問題 11
profile = {"name": "Ken", "age": 22} の'age'を30に変更

**解答:**
```python
profile = {"name": "Ken", "age": 22}
profile['age'] = 30
print(profile)  # {'name': 'Ken', 'age': 30}
```

**解説:**
- 既存のキーに新しい値を代入すると値が更新されます
- 辞書は可変オブジェクトなので直接変更可能
- キーが存在しない場合は新しいキー・値ペアが追加されます

## 問題 12
person = {"name": "Kenta"} に'gender':'male'を追加

**解答:**
```python
person = {"name": "Kenta"}
person['gender'] = 'male'
print(person)  # {'name': 'Kenta', 'gender': 'male'}
```

**解説:**
- 新しいキーに値を代入すると辞書に追加されます
- 他の追加方法: `person.update({'gender': 'male'})` や `person.setdefault('gender', 'male')`
- `setdefault()` はキーが既に存在する場合は値を変更しません

## 問題 13
person = {"name": "Yui", "age": 27, "city": "Osaka"} から'age'を削除

**解答:**
```python
person = {"name": "Yui", "age": 27, "city": "Osaka"}
del person['age']
print(person)  # {'name': 'Yui', 'city': 'Osaka'}
```

**解説:**
- `del 辞書[キー]` でキー・値ペアを削除します
- キーが存在しない場合は `KeyError` が発生
- 他の削除方法: `person.pop('age')` - 削除した値を返す
- 安全な削除: `person.pop('age', None)` - キーがない場合は `None` を返す

## 問題 14
fruit_prices = {"apple": 100, "banana": 80, "orange": 120} からすべてのキーを取得

**解答:**
```python
fruit_prices = {"apple": 100, "banana": 80, "orange": 120}
print(list(fruit_prices.keys()))  # ['apple', 'banana', 'orange']
```

**解説:**
- `keys()` メソッドは辞書のすべてのキーを取得します
- 戻り値は辞書ビューオブジェクト（dict_keys）
- リストに変換するには `list()` を使用
- Python 3.7以降は挿入順序が保持されます

## 問題 15
fruit_prices = {"apple": 100, "banana": 80, "orange": 120} からすべての値を取得

**解答:**
```python
fruit_prices = {"apple": 100, "banana": 80, "orange": 120}
print(list(fruit_prices.values()))  # [100, 80, 120]
```

**解説:**
- `values()` メソッドは辞書のすべての値を取得します
- 戻り値は辞書ビューオブジェクト（dict_values）
- 値は重複する可能性があります
- 直接反復処理も可能: `for value in fruit_prices.values():`

## 問題 16
fruit_prices = {"apple": 100, "banana": 80, "orange": 120} からすべてのキーと値を取得

**解答:**
```python
fruit_prices = {"apple": 100, "banana": 80, "orange": 120}
print(list(fruit_prices.items()))  # [('apple', 100), ('banana', 80), ('orange', 120)]
```

**解説:**
- `items()` メソッドはキー・値ペアのタプルを取得します
- 戻り値は辞書ビューオブジェクト（dict_items）
- ループでよく使用: `for key, value in fruit_prices.items():`
- タプルのアンパッキングで個別に取得可能

## 問題 17
items = {"apple": 3, "orange": 5} でキー'banana'が存在するか確認

**解答:**
```python
items = {"apple": 3, "orange": 5}
print('banana' in items)  # False
```

**解説:**
- `in` 演算子で辞書にキーが存在するかチェックできます
- 値ではなくキーをチェックします
- 値の存在確認: `'banana' in items.values()`
- より安全なアクセス: `items.get('banana')` でキーがない場合は `None`

## 問題 18
ネストした辞書からキー'math'の点数を取得

**解答:**
```python
student = {
    "name": "Tom",
    "scores": {
        "math": 90,
        "english": 80
    }
}
print(student['scores']['math'])  # 90
```

**解説:**
- ネストした辞書は連続した `[]` でアクセスします
- `student['scores']` で内側の辞書を取得、さらに `['math']` で値を取得
- 安全なアクセス: `student.get('scores', {}).get('math', 0)`
- 深いネストの場合は存在チェックが重要

## 問題 19
scores = {"A": 88, "B": 92, "C": 75} で最も値が大きいキーを取得

**解答:**
```python
scores = {"A": 88, "B": 92, "C": 75}
max_key = max(scores, key=scores.get)
print(max_key)  # B
```

**解説:**
- `max()` 関数の `key` パラメータで比較基準を指定
- `scores.get` は各キーの値を取得する関数
- 最大値も取得: `max_value = scores[max_key]`
- 最小値のキー: `min(scores, key=scores.get)`

## 問題 20
数値 10,20,30からなるタプルを作成

**解答:**
```python
my_tuple = (10, 20, 30)
print(my_tuple)  # (10, 20, 30)
```

**解説:**
- タプルは `()` で作成します
- 要素が1つの場合は `(10,)` のようにカンマが必要
- 空のタプル: `empty_tuple = ()`
- タプルは不変（immutable）オブジェクトです

## 問題 21
data = ("apple", "banana", "cherry") から2番目の要素を取得

**解答:**
```python
data = ("apple", "banana", "cherry")
print(data[1])  # banana
```

**解説:**
- タプルもリストと同様にインデックスでアクセスします
- インデックスは0から始まります
- 負のインデックスも使用可能: `data[-1]` で最後の要素
- スライスも可能: `data[1:3]` で部分取得

## 問題 22
nums = (5, 10, 15, 20) の要素数を取得

**解答:**
```python
nums = (5, 10, 15, 20)
print(len(nums))  # 4
```

**解説:**
- `len()` 関数でタプルの要素数を取得
- 空のタプルの場合は0を返します
- ネストしたタプルの場合、最上位レベルの要素数のみカウント

## 問題 23
point = (3, 7, 9) を3つの変数に分解

**解答:**
```python
point = (3, 7, 9)
x, y, z = point
print(x)  # 3
print(y)  # 7
print(z)  # 9
```

**解説:**
- タプルアンパッキング（分解代入）で複数変数に一度に代入
- 変数の数とタプルの要素数は一致させる必要があります
- 余った要素は `*` で受け取り可能: `x, y, *rest = point`
- 関数の戻り値でよく使用されます

## 問題 24
fruits = ("apple", "banana", "orange") に'banana'が含まれているか判定

**解答:**
```python
fruits = ("apple", "banana", "orange")
print('banana' in fruits)  # True
```

**解説:**
- `in` 演算子でタプル内の要素の存在を確認
- 線形探索で検索されるため、大きなタプルでは時間がかかる場合があります
- 存在しない場合は `False` を返します
- インデックス取得: `fruits.index('banana')` で位置を取得可能

## 問題 25
data = (1, 2, 3, 4, 5, 6) から前半3つの要素を取得

**解答:**
```python
data = (1, 2, 3, 4, 5, 6)
print(data[:3])  # (1, 2, 3)
```

**解説:**
- タプルでもリストと同様にスライス記法が使用可能
- `[:3]` は先頭から3番目の要素まで（3番目は含まない）
- 後半取得: `data[3:]` で4番目以降すべて
- 戻り値も新しいタプルになります

## 問題 26
a = (1, 2) と b = (3, 4) を結合

**解答:**
```python
a = (1, 2)
b = (3, 4)
combined = a + b
print(combined)  # (1, 2, 3, 4)
```

**解説:**
- `+` 演算子でタプル同士を結合できます
- 新しいタプルが作成されます（元のタプルは変更されません）
- 複数のタプルも結合可能: `a + b + c`
- 空のタプルとの結合も可能: `a + ()`

## 問題 27
t = ("a", "b") を3回繰り返し

**解答:**
```python
t = ("a", "b")
repeated = t * 3
print(repeated)  # ('a', 'b', 'a', 'b', 'a', 'b')
```

**解説:**
- `*` 演算子でタプルを指定回数繰り返し
- 新しいタプルが作成されます
- 0回繰り返し: `t * 0` で空のタプル `()` が作成
- 負の数の場合も空のタプルになります

## 問題 28
numbers = (4, 1, 9, 3, 7) の最大値と最小値を求める

**解答:**
```python
numbers = (4, 1, 9, 3, 7)
print(f"最大値: {max(numbers)}")  # 最大値: 9
print(f"最小値: {min(numbers)}")  # 最小値: 1
```

**解説:**
- `max()` と `min()` 関数でタプルの最大値・最小値を取得
- 数値以外でも比較可能な要素なら使用可能
- 空のタプルの場合は `ValueError` が発生
- 合計値: `sum(numbers)` で要素の合計も取得可能

## 問題 29
fruits = ("apple", "banana", "apple", "orange", "apple") で'apple'の出現回数

**解答:**
```python
fruits = ("apple", "banana", "apple", "orange", "apple")
print(fruits.count('apple'))  # 3
```

**解説:**
- `count()` メソッドで指定要素の出現回数を取得
- 存在しない要素の場合は0を返します
- 大文字小文字は区別されます
- すべての要素に対して線形探索が行われます

## 問題 30
nested = (("A", "B"), ("C", "D")) から'C'を取得

**解答:**
```python
nested = (("A", "B"), ("C", "D"))
print(nested[1][0])  # C
```

**解説:**
- ネストしたタプルは連続した `[]` でアクセス
- `nested[1]` で2番目のタプル `("C", "D")` を取得
- さらに `[0]` で最初の要素 `"C"` を取得
- 深いネストの場合も同様にチェーンできます

## 問題 31
a = 10, b = 20 をタプルを使用して交換

**解答:**
```python
a = 10
b = 20
a, b = b, a  # タプルを使った交換
print(f"a = {a}, b = {b}")  # a = 20, b = 10
```

**解説:**
- タプルアンパッキングを使った値の交換
- 右辺で `(b, a)` のタプルを作成し、左辺で `a, b` に展開
- 一時変数が不要で簡潔に書けます
- 3つ以上の値も同様に交換可能: `a, b, c = c, a, b`

## 問題 32
整数 1,2,3,4 を要素とするセットを作成

**解答:**
```python
my_set = {1, 2, 3, 4}
print(my_set)  # {1, 2, 3, 4}
```

**解説:**
- セットは `{}` で作成します（辞書とは異なり、キー・値ペアではない）
- 要素の重複は自動的に排除されます
- 要素の順序は保証されません（Python 3.7以降は挿入順序を維持）
- 空のセット: `set()` （`{}` は空の辞書になるため注意）

## 問題 33
[1,2,2,3,3,3,4] から重複を削除したセットを作成

**解答:**
```python
my_list = [1, 2, 2, 3, 3, 3, 4]
unique_set = set(my_list)
print(unique_set)  # {1, 2, 3, 4}
```

**解説:**
- `set()` 関数でリストからセットを作成
- 重複要素は自動的に1つだけ残されます
- リストに戻す場合: `list(unique_set)`
- 順序を保持して重複削除: `list(dict.fromkeys(my_list))`

## 問題 34
s = {1, 2, 3} に5を追加

**解答:**
```python
s = {1, 2, 3}
s.add(5)
print(s)  # {1, 2, 3, 5}
```

**解説:**
- `add()` メソッドで要素を1つ追加
- 既に存在する要素を追加しても変化しません
- 複数要素追加: `s.update([6, 7, 8])` や `s.update({6, 7, 8})`
- セットは可変オブジェクトです

## 問題 35
s = {1, 2, 3} から2を削除

**解答:**
```python
s = {1, 2, 3}
s.remove(2)
print(s)  # {1, 3}
```

**解説:**
- `remove()` メソッドで要素を削除
- 要素が存在しない場合は `KeyError` が発生
- 安全な削除: `s.discard(2)` - 要素がなくてもエラーにならない
- ランダム削除: `s.pop()` - 任意の要素を削除して返す

## 問題 36
s = {5, 10, 15} に10が含まれているか確認

**解答:**
```python
s = {5, 10, 15}
print(10 in s)  # True
```

**解説:**
- `in` 演算子でセット内の要素の存在を確認
- セットは高速な存在確認が可能（ハッシュテーブル使用）
- リストよりも大幅に高速（O(1) vs O(n)）
- 大量データの存在確認にはセットが効率的

## 問題 37
A = {1, 2, 3} と B = {3, 4, 5} の和集合

**解答:**
```python
A = {1, 2, 3}
B = {3, 4, 5}
union = A | B  # または A.union(B)
print(union)  # {1, 2, 3, 4, 5}
```

**解説:**
- 和集合：両方のセットの全要素（重複なし）
- 演算子 `|` またはメソッド `.union()` を使用
- 複数セット: `A | B | C` や `A.union(B, C)`
- 元のセットは変更されません

## 問題 38
A = {1, 2, 3} と B = {2, 3, 4} の積集合

**解答:**
```python
A = {1, 2, 3}
B = {2, 3, 4}
intersection = A & B  # または A.intersection(B)
print(intersection)  # {2, 3}
```

**解説:**
- 積集合：両方のセットに共通する要素
- 演算子 `&` またはメソッド `.intersection()` を使用
- 共通要素がない場合は空のセット `set()` を返す
- 複数セット: `A & B & C`

## 問題 39
A = {1, 2, 3, 4} と B = {3, 4, 5} の差集合

**解答:**
```python
A = {1, 2, 3, 4}
B = {3, 4, 5}
difference = A - B  # または A.difference(B)
print(difference)  # {1, 2}
```

**解説:**
- 差集合：AにあってBにない要素
- 演算子 `-` またはメソッド `.difference()` を使用
- 順序重要：`A - B` と `B - A` は異なる結果
- 複数セット: `A - B - C`

## 問題 40
A = {1, 2, 3} と B = {3, 4} の対称差

**解答:**
```python
A = {1, 2, 3}
B = {3, 4}
symmetric_diff = A ^ B  # または A.symmetric_difference(B)
print(symmetric_diff)  # {1, 2, 4}
```

**解説:**
- 対称差：どちらか一方のセットにのみ存在する要素
- 演算子 `^` またはメソッド `.symmetric_difference()` を使用
- 共通要素は除外されます
- 和集合から積集合を除いた結果と同じ：`(A | B) - (A & B)`

## 問題 41
colors = {"red", "green", "blue"} の要素を1行ずつ表示

**解答:**
```python
colors = {"red", "green", "blue"}
for color in colors:
    print(color)
# red
# green
# blue
```

**解説:**
- セットもforループで反復処理可能
- 要素の順序は保証されません（実装に依存）
- ソートして表示: `for color in sorted(colors):`
- セットは効率的な反復処理が可能

## 問題 42
items = {1, 2, 3, 4, 5} の要素数を取得

**解答:**
```python
items = {1, 2, 3, 4, 5}
print(len(items))  # 5
```

**解説:**
- `len()` 関数でセットの要素数を取得
- 重複がないため、ユニークな要素数がわかります
- 空のセットの場合は0を返します
- リストから重複除去後の要素数: `len(set(my_list))`

## 問題 43
n番目の要素の値がn*nであるリストを内包表記で作成（要素数10）

**解答:**
```python
squares = [n * n for n in range(1, 11)]
print(squares)  # [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
```

**解説:**
- リスト内包表記：`[式 for 変数 in イテラブル]`
- `range(1, 11)` で1から10までの数値を生成
- `n * n` で各数値の二乗を計算
- 従来の書き方と比較して簡潔で高速
- 条件付き内包表記：`[n*n for n in range(1, 11) if n % 2 == 0]` （偶数のみ）