# Branchs
São ramificaçoes do projeto, o qual permite varios desenvolvedores, trabalharem em diferentes funcionalidades, sem bugar a versão estável.

## Principais Branchs
Brench main -> que é a brench principal, ou seja, a brench estável da aplicação. Versão que é disponibilizada aos clientes.

Brench developer -> é a branch utilizada pelos testers. Os quais vão testar as novas funcionalidades, correções de bugs, etc.

## Outras Branchs
Para cada nova funcionalidade ou correção de bugs é criada uma nova brench.

### Padroes para criar nomes de branchs
!IMPOTANTE! Nomes de branchs não tem acento nem Ç

Para correção de bugs: fix_identificacao_do_bug
Exemplo: fix_botao_de_login, fix_cor_do_cabecalho

Para novas funcionalidades:
feat_identificacao_da_nova_funcionalidade
Exemplo: feat_integracao_com_google, feat_nova_tela_de_contato

Para atualizar documentação: doc_identificacao_da_alteracao
Exemplo: doc_adicionada_nova_imagem

Para criacao/alteracao de tarefas que nao interfere no codigo:
chore_identificacao_da_modificacao
Exemplo: chore_atualizado_a_versao_do_banco

## Criacao de novas branchs
git checkout -b nome_da_nova_branch
Exemplo: git checkout -b fix_botao_da_tela_login
Obs: O ideal é sempre criar as branchs a partir da main

### Listar as branchs existentes
git branch list

### Trocar de branch
git switch nome_da_branch_que_deseja_entrar
Exemplo 01: git switch fix_botao_da_tela_login
Exemplo 02: git switch main

### Excluir uma branch
git branch -D nome_da_branch_que_deseja_excluir
Exemplo: git branch -D fix_botao_da_tela_login

### Alterar o nome de uma Branch
Primeiramente, precisa estar dentro da branch e depois usar o comando para renomear.
git branch -m novo_nome_da_branch.

### Trazer as alterações de uma BRANCH para a MAIN

Primeiro, certifique-se que esta dentro da branch main. Se não estiver use: 
git switch main.

Segundo, verifique se a branch main esta atualizada com o comando:
git pull origin main.

Trazer os dados da branch para a main:
git merge nome_da_branch.