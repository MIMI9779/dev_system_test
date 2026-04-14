# コンテナ・バージョン管理・LLM練習用リポジトリ

## codespace 作成直後にやること
1. 仮想環境を導入してローカルLLM・Bonsaiのセットアップ
```Bash
git clone https://github.com/PrismML-Eng/Bonsai-demo.git
cd Bonsai-demo
uv venv
source .venv/bin/activate
uv pip install openai
BONSAI_MODEL=1.7B
./setup.sh
```
  - git cloneで, BonsaiのリポジトリからBonsai一式を落としてくる
  - cd Bonsai-demo で落としてきたBonsaiのフォルダに移動
  - uvで仮想環境venvを作成
    - 仮想環境下じゃないと, openaiを入れられない
  - source .venv/bin/activateで仮想環境venvに入る
  - uv pip install openaiで仮想環境下にopenaiライブラリをインストール
  - BONSAI_MODEL=1.7Bで, 利用するBonsaiのパラメタ数を1.7Bにする
