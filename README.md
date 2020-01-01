# bash_profile
My Bash Profile Setting

vi ~/.bash_profile
```sh
alias k=kubectl
alias kgp='k get po'
alias kgd='k get deploy'
alias h='history | grep'
alias g='git'
alias gcommit='g commit -m'
set -o vi
alias ll='ls - lG'
source <(kubectl completion bash)
echo "source <(kubectl completion bash)" >> ~/.bashrc
complete -F __start_kubectl k
```
