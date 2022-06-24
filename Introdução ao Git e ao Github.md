# Módulo 1



## Introdução ao GitHub

#### Comandos básicos para um bom desempenho no terminal:

GUI [graphic user interface] x CLI [common line interface]

#### Navegação do GIT no Windows:

Lista de alguns comandos:

- cd / [navegação entre pastas]

- dir [diretórios/pastas]

- mkdir [criação de diretórios/pastas]

- del / rmdir [deleta diretório]

- cd .. [voltar]

- ctrl+l; clear [limpar o terminal]

- echo [printa uma palavra e coloca num arquivo]

- de/rmdir [remover diretório]

- rf [apagar todas as pastas]

- git clone [clona um código privado no github]

- -a [revela pastas ocultas]

- git init [cria um diretório]

- git add . [adiciona um commit]

- git push origin main [envia para o github]

  

  ## Tópicos fundamentais para entender o funcionamento do Git 

  O SHA1 [secure hash algorithm]: é um conjunto de funções hash criptográficas projetadas pela NSA [agência de segurança nacional dos EUA]; a encriptção gera um conjunto de caracteres de 40 dígitos. Ele é uma forma curta de representar um arquivo. 

#### Objetos internos do git

1. BLOBS 
Os arquivos são guardados no blobs [contém metadados].  No blob contém o tipo, tamanho, uma barra com o 0 e o conteúdo do arquivo. Ela tem o sha1 do arquivos. 

2. TREE
Elas armazenam as blobs. Ela também contém metadados. Ela é responsável por montar a estrutura de onde estão os arquivos. Elas tem o sha1 dos metadados.

EXEMPLO:
                      
                        Tree

readme           rakefile             lib
      |                       |                   | 
  blob                 blob            simplegit.rb
                                                    |
                                                  blob

COMMIT:
Ele aponta para o tree, parente, autor e mensagem. Ele tem um timestamp [horário e data]; Possui um sha1 e encriptação.

Nota: Sistema distribuído seguro



## Chave SSH e Token

A chave SSH é uma forma segura de estabelecer uma conexão segura para outra máquina.

## Iniciando o git e criando um commit

- Git init: cria um repositório
- Git add: salva alterações
- Git commit: capturam o estado atual do projeto
- Git status: verifica o status do repositório

## Passo a passo no ciclo de vida

Repositório: 
- Servidor: remote repository 

Ambiente de desenvolvimento:
- Working directory
- Staging area
- Local repository

Tracked: unmodified; modified; staged 

Onde fica os arquivos que se preparam para fazer parte de outro agrupamento.

Untracked: 

adiciona arquivo; edita arquivo; ''stage'' o arquivo; remove o arquivo; commit.