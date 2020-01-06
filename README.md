# mac-brew-ansible

### 準備
1. `Xcode` インストール
2. `Homebrew` インストール
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
3. `ansible` インストール
```
brew install ansible
```
4. シェル設定ファイル（ `./bashrc` 、 `./zshrc` 等） に下記追加
```
export HOMEBREW_CASK_OPTS="--appdir=/Applications"
```

### cloneしてplaybook実行
```
# clone （ `setup` ディレクトリにcloneする例 ）
cd ~
git clone https://github.com/tamken/mac-brew-ansible.git setup


# 実行
cd ~/setup
ansible-playbook setup.yml -i inventory 
```
