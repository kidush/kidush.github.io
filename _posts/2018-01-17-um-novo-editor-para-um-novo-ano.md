---
layout: post
title: "Um “novo” editor para um novo início de ano"
date: 2018-01-17 21:59:26 -0300
category: environment,emacs,vim,from-medium
published: false
---

*****

É de praxe que todo ano que está para se iniciar, toda pessoa no mundo faz
milhares e milhares de promessas e metas para o novo ano que está iniciando. E
eu não sou diferente, estou com algumas metas em mente e estou me organizando o
máximo para não falhar com elas. Mas como esse post é sobre um editor e não
sobre minhas metas, vamos mudar de assunto rsrs.

Pra começar bem decidi começar o ano usando um editor temido e amado por muitos
chamado [Emacs](http://www.gnu.org/software/emacs/).

*****

### Como cheguei até aqui?

Passei metade de 2016 e todo 2017 usando VIM em tudo que eu precisasse escrever
no meu trabalho e fora também. Já usei e testei vários editores de texto como
[Sublime Text](https://www.sublimetext.com/), [Atom](https://atom.io/), [Visual
Studio Code](https://code.visualstudio.com/) e outros mais. Claro, todos em modo
VI. Fazia um bom tempo que estava pensando em testar o Emacs, mas não queria
perder muitas horas aprendendo os atalhos do emacs e configurando ele até ficar
do jeito que eu queria.

Então, começei a procurar modos de como utilizar o VIM dentro do Emacs e nessa
procura terminei encontrando o
[evil-mode](https://www.emacswiki.org/emacs/Evil). Infelizmente ainda assim
teria que me adequar a Leader key do Emacs e configurá-lo. E era justamente o
que eu não queria. Continuei procurando mais um pouco na internet e encontrei o
[Spacemacs](http://spacemacs.org/) e é sobre ele que quero escrever um pouco 😄.

*****

### Primeiramente… O que é o Spacemacs?

![](https://cdn-images-1.medium.com/max/800/1*SMllGduhDrQMZ0zb1o_iQg.png)
<span class="figcaption_hack">Python layer on spacemacs</span>

Basicamente ele é uma distribuição do Emacs mantida pela comunidade opensource.
Ele é bem intuitivo e com atalhos fáceis de decorar, foi criado para pessoas que
como eu, usuários **vim**, tem interesse em ter todo o poder do Emacs junto do
**vim** com uma curva de aprendizado bem menor do que se você fosse migrar para
o Emacs padrão.

Mesmo tendo os usuários do **vim** como usuários “principais” ele se adequa a
qualquer tipo de usuário. Nele você pode utilizar tanto o evil-mode que citei
logo no começo, como o modo padrão do emacs ou um modo Híbrido(Emacs e Vim).

Se você quer usar o evil-mode assim como eu, mas também não sabe nada de **vim**
dentro do spacemacs você tem um evil-tutor, que nada mais é do que um tutorial
pra quem ta começando com o **vim.**

Acessando o evil-tutor. Mais abaixo irei falar mais de alguns atalhos.


#### Os Pilares Principais do Spacemacs

* Mnemonico (Te ajuda a decorar facilmente os atalhos)
* Intituitivo (Tem um display maravilhoso, como todos os atalhos)
* Consistente (Em todo lugar que utilizar o spacemacs, terá os mesmos atalhos)
* Guiado pela Comunidade (Layers para tudo que você imaginar 😸)

*****

### Configuration Layers

Pra quem vem do mundo **vim** estamos acostumados com os milhares de plugins que
exsistem para ele. No **spacemacs **são chamados de Layers e alguns bem úteis já
vem configurados por padrão e são muito mais fáceis e rápidos pra instalar.

Para adicionar layers nele é bem intuitvo. Logo abaixo irei mostrar o processo
de instalação e algumas modificações que fiz para meu uso 😆

### Então… vamos instalá-lo

Como estou no Linux(Ubuntu) e já tinha o emacs instalado, o processo foi
basicamente clonar o repositório do spacemacs para a minha pasta de configuração
do emacs **~/.emacs.d**. Na documentação tem explicando, mas vou deixar aqui pra
facilitar.

Rode o comando abaixo assim que você tiver o emacs instalado em sua máquina.
Caso não tenha ele instalado ainda, recomendo usar o emacs 25 por ser mais
recente.

    git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d

para instalar emacs no Mac OS e no Windows deixarei o link logo abaixo do
próprio repositório do spacemacs.

* [Instalando no Windows](https://github.com/syl20bnr/spacemacs#windows)
* [Instalando no Mac OS](https://github.com/syl20bnr/spacemacs#macos)

### Layers que utilizo e alguns atalhos básicos

Como falei acima, os atalhos dele são bem intuitivos e ajuda-nos a decorar a
maioria dos comandos dentro do editor.

No vim geralmente utilizariamos a `,` como Leader key, o Spacemacs utiliza
uma Leader key bem mais intuitiva que é o espaço(SPC).

Por exemplo, para você editar ou criar um novo arquivo nele é só digitar:

    SPC - f - f

Para instalar novos layers ou para fazer qualquer outra modificação no editor é
só ir no nosso arquivo dotfile **~/.spacemacs.**

> Dentro deste arquivo fica todas as configurações que você pode mexer dentro do
> editor.

#### Acessando o arquivo de configuração:

    SPC - f - e - d

![](https://cdn-images-1.medium.com/max/1600/1*lb0PLY7FuhStXfRupiLyxw.png)
<span class="figcaption_hack">.spacemacs file</span>

> Ele é um arquivo lisp, mas não se assuste é fácil de editar e entender, o
> arquivo está bem comentado 😄

#### Os layers que estou utilizando hoje são:

* Python
* Ruby
* Javascript
* helm
* auto-completion
* yaml
* html
* git
* E mais alguns 😆

#### **Lista de layers disponíveis na documentação:**
[Layers do spacemacs](http://spacemacs.org/layers/LAYERS.html)

### Temas

Ele já vem com uma lista de temas pré-instalados, para acessar a lista só
digitar o seguinte atalho.


Mas como falei acima, existem diversos layers criados pela comunidade e um legal
que encontrei recentemente foi o **themes-megapack.**

para instá-lo basta adicioná-lo ao seu **~/.spacemacs**


Ao abrir vá até o seu dotspacemacs-configuration-layers. Na imagem abaixo você
verá no final o **themes-megapack.**

<span class="figcaption_hack">dotspacemacs-configuration-layers. Alguns dos layers que tenho instalado</span>

Após isso você precisará recarregar o editor, para ele instalar os pacotes.


Quando o processo terminar o spacemacs precisará ser reiniciado.


Assim que você abrir a lista de temas.


Você verá que novos temas foram instalados. Hoje estou utilizando o spacegray
como na imagem logo abaixo.

<span class="figcaption_hack">org-mode com o tema do spacegray.</span>

*****

### Quase iria esquecendo do Terminal

Ele também tem um ótimo terminal integrado assim como todo editor decente
deveria ter. 😃

O bom é que faço praticamente tudo dentro do Emacs(Spacemacs). Como utilizo
muito o terminal não preciso ta saindo de dentro do editor para rodar algum
comando no sistema operacional.

Abrindo o terminal:


<span class="figcaption_hack">terminal dentro do spacemacs</span>

### Finalizando…

Então, como só queria mostrar um pouco de como estou amando trabalhar com o
spacemacs, vou parando por aqui, futuramente pretendo mostrar mais como
funcionam os modes e como estes modes tem me ajudado a organizar minha vida como
Desenvolvedor.

Por exemplo, nele você consegue criar apresentações, exportar estas
apresentações para html, lateX, criar TODO lists, agendas e por ai vai. Como
dizem os usuários a mais tempo que eu.

> O Emacs é um ótimo sistema operacional e um editor decente.

Espero ter tempo para continuar escrevendo sobre minha experiência no dia-a-dia
com este editor e irei postando as atualizações por aqui. Até mais pessoal.

* [Development](https://medium.com/tag/development?source=post)
* [Emacs](https://medium.com/tag/emacs?source=post)
* [Environment](https://medium.com/tag/environment?source=post)
* [Vim](https://medium.com/tag/vim?source=post)

By clapping more or less, you can signal to us which stories really stand out.

### [Thiago Ferreira](https://medium.com/@thiagoflins)
