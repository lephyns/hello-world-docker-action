# hello-world-docker-action


$ chmod +x entrypoint.sh


Em seu diretório hello-world-docker-action, crie um arquivo README.md que especifique as seguintes informações:

• Uma descrição detalhada do que a ação faz.

• Argumentos de entrada e saída necessários.

• Argumentos de entrada e saída opcionais.

• Segredos que a ação usa.

• Variáveis de ambiente que a ação usa.

• Um exemplo de como usar sua ação em um fluxo de trabalho.

README.md
# Ação do docker “Hello World”

Esta ação imprime "Hello World" ou "Hello" + o nome de uma pessoa para saudar no log.

## Entradas / Inputs

## `quem cumprimentar`

**Obrigatório** O nome da pessoa a ser cumprimentada. Padrão `"Mundo"`.

## Saídas

## `hora`

A hora em que te cumprimentamos.

## Exemplo de uso

uses: actions/hello-world-docker-action@v1
with:
   who-to-greet: Carlos Oliveira


É uma prática recomendada adicionar também uma tag de versão para lançamentos de sua ação.

Shell
git add action.yml entrypoint.sh Dockerfile README.md
git commit -m "My first action is ready"
git tag -a -m "My first action release" v1
git push --follow-tags


O código de fluxo de trabalho a seguir usa a ação hello world concluída no repositório public actions/hello-world-docker-action. Clique em “Actions” e depois em “Configure” no item Manual Workflow (Automation items). Copie o código de exemplo de fluxo de trabalho a seguir em um arquivo .github/workflows/main.yml, mas substitua actions/hello-world-docker-action pelo seu repositório e nome da ação. 