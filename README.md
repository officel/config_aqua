# .config/aqua

- [CLI バージョン管理ツールの aqua を使うようになって少し経ったので少しまとめておく](https://zenn.dev/raki/articles/2024-05-16_aqua)

## note

.bash_profile あたりに

```bash
# cli version manager aqua
# export AQUA_GLOBAL_CONFIG="$HOME/.dotfiles/aqua/aqua.yaml"
export AQUA_GLOBAL_CONFIG="$HOME/.config/aqua/aqua.yaml"
export PATH="$(aqua root-dir)/bin:$PATH"
```
