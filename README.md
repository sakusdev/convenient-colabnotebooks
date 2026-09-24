# 便利な Colab ノートブック

Google Colab で開いて、上から順に実行できる小さな道具をまとめています。ノートブックは日本語で説明し、入力ファイルを勝手に上書きしない構成にしています。

| ノートブック | できること | 入力 → 出力 |
| --- | --- | --- |
| [実行環境チェック](notebooks/colab_runtime_diagnostics.ipynb) · [Colab で開く](https://colab.research.google.com/github/sakusdev/convenient-colabnotebooks/blob/main/notebooks/colab_runtime_diagnostics.ipynb) | GPU、VRAM、RAM、空き容量、PyTorch、指定したライブラリを確認 | 実行環境 → 画面表示、任意の JSON |
| [CSV / Excel の確認と整理](notebooks/csv_excel_inspector_cleaner.ipynb) · [Colab で開く](https://colab.research.google.com/github/sakusdev/convenient-colabnotebooks/blob/main/notebooks/csv_excel_inspector_cleaner.ipynb) | 列型、欠損、重複を確認し、選んだ処理だけ適用 | CSV / XLSX → 別名の CSV |
| [画像を一括リサイズ・形式変換](notebooks/画像を一括リサイズ・形式変換.ipynb) · [Colab で開く](https://colab.research.google.com/github/sakusdev/convenient-colabnotebooks/blob/main/notebooks/%E7%94%BB%E5%83%8F%E3%82%92%E4%B8%80%E6%8B%AC%E3%83%AA%E3%82%B5%E3%82%A4%E3%82%BA%E3%83%BB%E5%BD%A2%E5%BC%8F%E5%A4%89%E6%8F%9B.ipynb) | 向き補正、縮小、WebP / JPEG / PNG への一括変換 | 画像 → 変換画像をまとめた ZIP |

## 使い方

1. 表の「Colab で開く」を押します。Google アカウントでログインが必要です。
2. 上から順にセルを実行し、設定があるセルは必要に応じて変更します。
3. ファイルを扱うノートブックではブラウザーからファイルをアップロードし、結果をダウンロードします。Colab の一時領域はセッション終了で消えるため、必要な結果は手元に保存してください。

ノートブックを実行する前に各セルの内容を確認してください。入力データや診断結果に個人情報が含まれる場合は、共有時にも内容を確認してください。

## 追加・修正するとき

- 説明と実行セルを上から順に並べ、初期設定で元ファイルを削除・上書きしないようにします。
- Notebook の実行結果やアップロードした私的ファイルはコミットせず、`.ipynb` のセル出力を空にします。
- CPU ランタイムでも使える場合は GPU の有無を確認し、必要な追加パッケージがある場合はセル内で明示します。
