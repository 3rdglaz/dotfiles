# mini passo a passo

pela enesima vez eu começo a configurar um linux do nada

## WM - i3

[config](https://github.com/3rdglaz/dotfiles/blob/master/.config/i3/config)
  
## StatusBar - polybar

[config](https://github.com/3rdglaz/dotfiles/blob/master/.config/polybar/config)

## BASH - zsh

	$ sudo apt install zsh

## PLUGIN

oh-my-zsh
https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

p10k
https://github.com/romkatv/powerlevel10k#oh-my-zsh

- tem que lembrar que no arquivo do zsh, tem que dar source
	`source /home/c/.oh-my-zsh/custom/themes/powerlevel10k/powerlevel10k.zsh-theme`

## FONT - ShureTechMono NF
	https://www.nerdfonts.com/font-downloads

## Xresource - 

copiei da internet, mas como não to usando o URXVT(por não aceitar fonte), acho irrelevante. EDIT: tem utilidade pra cores do sistema.

## Terminal - Gnome-Terminal

Gogh, simplesmente excelente pra baixar o tema e rodar num perfil padrão
https://github.com/Gogh-Co/Gogh

## Paleta de Cor - TokyoNight Storm

## Editor de Texto NeoVim

[config](https://github.com/3rdglaz/dotfiles/blob/master/.config/nvim/init.vim)

prerequisito: nodejs npm yarn

neovim já vem com gerenciador de plugins, então o .conf já funciona do 0, só dar

```
  :PlugInstall
  :call coc#util#install()
```

pra inserir um autocomplete é só usar algum Language Server(no git do COC), e seguir o passo a passo
A configuração pode ser acessado dentro do nvim com 

```
:CocConfic.
```

## LSD

https://github.com/Peltoche/lsd

[config](https://github.com/3rdglaz/dotfiles/blob/master/.config/lsd/config.yaml)

## BAT

https://github.com/sharkdp/bat

## Disabilitar Power Save Mode

Ve se tá ativo:

```
xset -q | awk '/DPMS is/ {print $NF}'
```


> xset -q | awk '/DPMS is/ {print $NF}'
> 
> Enabled

Desabilita:

```
xset -dpms
```

Habilita:

```
xset dpms
```
## Auto-Git-Commit

editar/add **~/.netrc**

```
machine github.com login {usr} password {senha}
```

fazer:
arrumar notificação do i3
