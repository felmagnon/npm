# NPM
Saiba o que é NPM (Node Package Manager) e como instalar
```
O NPM (Node Package Manager) é o Gerenciador de Pacotes do Node (interpretador Javascript do lado do servidor).
Trata-se de um repositório online para publicação de projetos de código aberto para o Node.js e também é um utilitário que interage com este repositório. Além dessas funções, o NPM auxilia na instalação de pacotes, no gerenciamento de versão e gerenciamento de dependências.  Sua instalação já ocorre quando se instala o Node.js.
```

## O que é NPM? 

O NPM é uma ferramenta do Node.js para o gerenciamento de pacotes. Ele permite instalar, desinstalar e atualizar dependências em uma aplicação por meio de uma simples instrução na linha de comando. Sempre que um projeto é criado por meio do gerenciador, é adicionado um arquivo chamado package.json, que contém a relação dos pacotes instalados no ambiente.

**Exemplo:** 
```
{
  "name": "automacao",
  "version": "1.0.0",
  "description": "automacao de testes para aplicação web",
  "main": "protractor.conf.js",
  "scripts": {
    "test": "protractor protractor.conf.js"
  },
  "author": "magnonSantos",
  "license": "ISC",
  "dependencies": {}
}
```
**Observação:** Assim, quando for preciso realizar alguma alteração, o NPM verifica esse arquivo e faz as atualizações necessárias de forma simples e rápida. Isso contribui para manter a organização do projeto e de suas dependências, além de evitar erros de configurações ao fazer a instalação de pacotes de forma manual.

## Por que devo usa-lo?

Realizar instalações manuais de bibliotecas, frameworks e ferramentas pode ser bem trabalhoso, além de ser maior as chances de realizar configurações erradas.

## Comandos básicos:
`npm -version` / `npm -v`: Exibi a versão do NPM.

`npm install` / `npm i`: Instalação dos módulos e dependências no projeto localmente.

`npm install --global` / `npm i -g`:  Instalação dos módulos e dependências no projeto globalmente.

`npm list` / `npm ls`: Lista todos os módulos localmente.

`npm list -g`: Lista todos os módulos globais.

`npm init`: Cria o arquivo `package.json` onde são armazenadas as dependências e outras configurações do projeto.

`npm list -save -dev`: Registra no arquivo `package.json` as dependências utilizadas durante o desenvolvimento.

`npm uninstall`: Desinstala o pacote do projeto.

`npm update` / `npm up`: Atualizará todos os pacotes listados para a versão mais recente e também pacotes ausentes.

## NPM em automação de testes

**Informativo:** Para utilizar o `npm` nos testes com o `protractor` é preciso garantir que o `node.js` está devidamente instalado, a forma mais simples de verificar isso é através do comando `node --version` com o `node.js` instalado podemos seguir os próximos passos.

`npm install protractor -g`: Instalação do `protractor` globalmente.

`npx webdriver-manager update`: Faz atualização do `chromedriver` e do `geckodriver(firefox)` com a versão mais recente do navegador.

`npm i`: Instalação de todas as depedências constantes no arquivo `package.json`.

`npm test` / `npm t`: Utilizado para executar os teste.





