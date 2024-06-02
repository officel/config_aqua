# .config/aqua

- [CLI バージョン管理ツールの aqua を使うようになって少し経ったので少しまとめておく](https://zenn.dev/raki/articles/2024-05-16_aqua)

## .bashrc

```bash
# cli version manager aqua
export PATH="$(aqua root-dir)/bin:$PATH"
export AQUA_GLOBAL_CONFIG=${XDG_CONFIG_HOME:-$HOME/.config}/aqua/aqua.yaml
```

## alias

```bash
alias aq='aqua'
alias aqcd="cd ${XDG_CONFIG_HOME:-$HOME/.config}/aqua/"
alias aqgi='aqua generate -i -o $AQUA_GLOBAL_CONFIG'
alias aqia='aqua install --all'
alias aqli='aqua list --installed --all | sort'
alias aqup='aqua update'

# global 配置の aqua を global 配置の task で一発アップデート
alias taskga='task -g a'
```

## direnv

- .direnv と .env で github token を設定した
- [Tips｜aqua CLI Version Manager 入門](https://zenn.dev/shunsuke_suzuki/books/aqua-handbook/viewer/tips#github_token%2C-aqua_github_token-%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%97%E3%81%A6-rate-limit-%E3%82%92%E5%9B%9E%E9%81%BF%E3%81%99%E3%82%8B)

# related my projects

- [officel/config_aqua: .config/aqua](https://github.com/officel/config_aqua)
- [officel/config_bash: .config/bash](https://github.com/officel/config_bash)
- [officel/config_git: .config/git](https://github.com/officel/config_git)
