# LinuxCommandPractice

# 様々なLinuxコマンド（調べたもの 復習 再提出）

```
LinuxCommandPracticeディレクトリ内から移動せずに、practice_dir_1内にpractice_dir_2というディレクトリを作成してください。但し、相対パスを使用してください。

mkdir practice_dir_1/practice_dir_2
```

```
practice_file1.txtを2つ上の階層のディレクトリ(LinuxCommandPractice)へ移動してください。但し、相対パスを使用してください。

mv practice_file1.txt ../../


mvコマンドでは、移動先のパスを正確に指定する必要。
実際には、現在のディレクトリから2つ上の階層（LinuxCommandPracticeディレクトリ）に移動するために、../../を使う事が重要。
```

```
次のコマンドを使用して、practice_file2.txtを2つ上の階層のディレクトリ（LinuxCommandPracticeディレクトリ）にコピー。

cp practice_file2.txt ../../

コピーもmvコマンド同様
```

```
次のコマンドを使用して、2つ上の階層のディレクトリ（LinuxCommandPracticeディレクトリ）に移動。


../..は、「親ディレクトリの親ディレクトリ」という意味
```

```
practice_dir_2ディレクトリを削除してください。但し、相対パスを使用してください。

rm -r practice_dir_1/practice_dir_2

rmには-f、-r、-iといったオプションが存在する。
rm -rはフォルダ（中に入っているファイルごと）消去。
rm -iは消去前に確認をすることができる。
rm -fはファイルが存在するかどうか関係なしに削除し、削除前の確認も行いません。
```

```

その後、iコマンドを打ちましょう。そうすると、INSERT, 編集モードへ移行します。
ファイルに、echo "Hello, World!"と記述してください。

vi practice_file1.txt



そして、エスケープボタンを押します。すると編集モードからコマンドモードに移行します。
最後に、:wqと打つと、保存されて編集が終了します。

i 編集モードへ移行
エスケープボタン コマンドモードへ移行
:w 一時保存
:q 保存せず終了
:q!強制終了
:wq 保存したのち終了
```