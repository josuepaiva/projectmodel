# projectmodel

Este projeto tem como objetivo ensinar programadores a configurar e usar a ferramenta editorconfig

## 1° Instalação

Para os seguintes editores não é necessário baixar plugin pois já existe suporte nativo.

* [BBEdit](http://www.barebones.com/support/technotes/editorconfig.html)
* [CodeCrusader](https://sourceforge.net/projects/codecrusader/)
* [Codelie](https://github.com/eranif/codelite/tree/master/EditorConfigPlugin)
* [IntellijCommunity](https://github.com/JetBrains/intellij-community/tree/master/plugins/editorconfig)
* [VisualCtudio](https://docs.microsoft.com/en-us/visualstudio/releasenotes/vs2017-relnotes-v15.0#coding-convention-support-through-editorconfig)
* [WebStorm](https://github.com/JetBrains/intellij-community/tree/master/plugins/editorconfig)

Para os seguintes editores é preciso baixar o plugin.

* [AppCode](https://plugins.jetbrains.com/plugin/7294-editorconfig)
* [Atom](https://github.com/sindresorhus/atom-editorconfig#readme)
* [Brackets](https://github.com/kidwm/brackets-editorconfig/)
* [Eclipse](https://github.com/ncjones/editorconfig-eclipse#readme)
* [Netbeans](https://github.com/welovecoding/editorconfig-netbeans#readme)
* [Notepad++](https://github.com/editorconfig/editorconfig-notepad-plus-plus#readme)
* [Sublime](https://github.com/sindresorhus/editorconfig-sublime#readme)
* [PhpStorm](https://plugins.jetbrains.com/plugin/7294-editorconfig)
* [VisualStudioCode](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

# 2° Configuração

Criar um arquivo na pasta do projeto chamado .editorconfig
A primeira propriedade escrita no arquivo serão

```javascript
root = true
```

Esta linha faz com que o editor pare de buscar outros arquivos de configuração

Regras que serão definidas

* Indentação deve ser feita com espaços
* Para cada indentação, deve ser dado quatro (4) espaços
* Utilizar o charset utf-8
* Não adicionar linhas em branco no final dos arquivos
* Apagar os espaços em brancos no final de cada linha

# Identação deve ser feita com espaços

```javascript
indent_style = space
```

# Para cada indentação, deve ser dado quatro (4) espaços
```javascript
indent_size = 4
```
# Utilizar o charset utf-8
```javascript
charset = utf-8
```

# Não adicionar linhas em branco no final dos arquivos
```javascript
insert_final_newline = false
```

# Apagar os espaços em brancos no final de cada linha
```javascript
trim_trailing_whitespace = true
```
# Definindo formatos de arquivos onde as configurações serão aplicadas
```javascript
[*] // O * é utilizado para dizer que serão aplicados em todos os tipos de arquivos
```

# Por fim o arquivo .editorconfig ficará assim:
```javascript
root = true
[*]
indent_style = space
indent_size = 4
charset = utf-8
insert_final_newline = false
trim_trailing_whitespace = true
```

# [Para mais detalhes acesse o site](https://blog.matheuscastiglioni.com.br/padronizando-seus-editores-de-texto-com-editorconfig)
