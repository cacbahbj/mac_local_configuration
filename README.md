# mac_local_configuration
Macの初期設定用ansibleファイル

PC購入時等のソフトウェア、ライブラリ導入用  
※わかりやすさ優先のためRoleを使用しない方法で記述しています  

以下で動作確認
- MacBook Pro 2021 / Apple M1 Pro
- ansible 2.16.7
- homebrew 4.3.5

## 事前準備

下記を参照してHomebrewをインストール  
https://brew.sh/ja/

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Ansibleをインストール
```
brew install ansible
```

## セットアップ

実行コマンド
```
ansible-playbook localhost.yml -i hosts -v
```

(変更せずにチェックだけする場合)
```
ansible-playbook localhost.yml -i hosts -v --check
```

## 参考

- Homebrew  
https://brew.sh/ja/
- Ansible Documentation  
https://docs.ansible.com/ansible/latest/
- mas-cli  
https://github.com/mas-cli/mas
