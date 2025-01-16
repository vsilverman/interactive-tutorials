入力を受け取り、必要な形式で出力を表示することは、対話型コーディングにおいて重要な役割を果たします。さっそく、さまざまなデータ型の入力と出力について焦点を当てましょう。

### raw_input()
これは、行の終わりに達するまで入力を受け取るために使用されます。スペースがあってはなりません。入力は改行文字によって終了し、入力行にスペースがあるとエラーになります。

    # 標準入力から受け取った入力を出力します
    astring=raw_input()# 入力としてhelloを与える
    print raw_input()

入力を受け取った後、int()、float()、str()のような関数を使って必要なデータ型に変換することができます。

    num=int(raw_input())
    print num
    decimalnum=raw_input()
    decimalnum=float(raw_input())
    print decimalnum

### input()
特に整数を入力するために使用されます。input()のraw_input()に対する利点は次の例で明らかになります。

    # 2*2を入力として与える
    a=input()
    b=raw_input() # int(raw_input())はエラーになることに注意
    print a # 4を出力
    print b # 2*2を出力

### どのようにして1行からスペースで区切られた2つ以上のデータ型を入力しますか？
ここではsplit()とmap()関数を使用します。

    # 1行目に2つの整数、3行目に2つ以上の整数を与える
    a, b = map(int, raw_input().split())
    array = raw_input().split()
    sum = 0
    for each in array:
        sum = sum + int(each)
    print(a, b, sum)  # 1行目の最初の2つの整数と2行目の整数の合計を出力

### 出力のフォーマット
print文が自動的に改行を挿入することに既に気付いているかもしれません。上記のコードでのコンマの使用は、スペースで区切られた単一行で値を出力します。
sysモジュールは出力フォーマットのための様々な関数を提供しますが、ここでは基本的なフォーマット知識を使用して必要な形式で出力する方法を学びます。いくつかの例を見て出力フォーマットを学びましょう。

    a = 5
    b = 0.63
    c = "hello"
    print "a is : %d, b is %0.4f,c is %s" % (a,b,c)

出力は自明であるべきです。

Exercise
--------

ユーザーに名前、年齢、および国名を入力するように求めるプログラムを書きなさい。その後、入力された情報を含むメッセージを文として出力します。プログラムは以下を含む必要があります：

1. 'raw_input()'を使用して名前を入力する。
2. 'input()'を使用して年齢を入力し、整数に変換する。
3. 'raw_input()'を使用して国名を入力する。
4. 名前、年齢、国を含む文を表示するように出力をフォーマットする。

プログラムはPythonでの入力ハンドリングと文字列フォーマットを実演する必要があります。