# Guia de Instalação do ZSH e Configuração do Oh My ZSH
Instalação do ZSH e Configuração do Oh My ZSH

O Z Shell (ZSH) é um shell poderoso que pode melhorar sua experiência de terminal com recursos avançados, como sugestões automáticas, destaque de sintaxe e muito mais. Oh My ZSH é um framework para gerenciar sua configuração ZSH, trazendo ainda mais funcionalidades através de temas e plugins. Este guia abordará a instalação do ZSH, Oh My ZSH e a configuração de alguns plugins úteis.
Instalação do ZSH

Para instalar o ZSH e os plugins de sugestões automáticas e destaque de sintaxe, execute o seguinte comando no terminal:

sudo apt install zsh-autosuggestions zsh-syntax-highlighting zsh

Este comando instalará o ZSH juntamente com os plugins de sugestões automáticas e destaque de sintaxe, proporcionando uma experiência de linha de comando aprimorada.
Instalação do Oh My ZSH

Oh My ZSH é uma estrutura comunitária que enriquece a experiência ZSH com uma configuração fácil e acesso a uma ampla variedade de temas e plugins. Para instalá-lo, execute:

bash

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

Este comando baixa e executa o script de instalação do Oh My ZSH, configurando-o como seu shell padrão.
Instalação de Plugins

A seguir, vamos instalar plugins adicionais para melhorar ainda mais sua experiência de terminal:

    autosuggestions plugin

    bash

git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

zsh-syntax-highlighting plugin

bash

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

zsh-fast-syntax-highlighting plugin

bash

git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting

zsh-autocomplete plugin

bash

    git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete

Habilitação de Plugins no .zshrc

Para ativar os plugins instalados, você precisa editar o arquivo de configuração .zshrc:

    Abra .zshrc com o editor de sua escolha (por exemplo, nvim ~/.zshrc).

    Localize a linha que diz plugins=(git).

    Substitua essa linha por:

    makefile

    plugins=(git zsh-autosuggestions zsh-syntax-highlighting fast-syntax-highlighting zsh-autocomplete)

Salve e feche o arquivo. Para que as alterações entrem em vigor, você pode reiniciar seu terminal ou executar source ~/.zshrc.

## References

 - [Oh my ZSH](https://github.com/ohmyzsh/ohmyzsh)
 - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
 - [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
 - [zsh-fast-syntax-highlighting](https://github.com/zdharma/fast-syntax-highlighting)
 - [zsh-autocomplete](https://github.com/marlonrichert/zsh-autocomplete)

