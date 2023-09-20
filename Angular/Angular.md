# ANGULAR

## Instalação do Node e NPM
- Instalar o Node e verificar a versão, verificar também a versão do NPM.

```
node --version
```
```
npm --version
```

## Instalação do CLI do angular
- Realizar a instalação por meio do prompt de comando
- disponível em: https://angular.io/guide/setup-local

```
npm install -g @angular/cli
```

## Extensões VSCode
- Angular Language Service
- Angular Snippets
- ESLint
- HTML CSS Support
- HTML Boilerplate
- IntelliCode

## Iniciando o projeto 

```
ng new my-app
```
- Logo em seguida ele perguntará se você deseja compartilhar informações e configurações com a Google, pode ser y/n
- E depois se deseja trabalhar com routings, que são basicamente os endereços que utilizamos em aulas passadas, como localhost:8080/alunos
- No stylesheet formater selecionar CSS.

---

## Rodando a aplicação
```
ng serve --open
```
- CTRL + C para parar a aplicação

- ## Criando novos componentes
```
ng generate componente nome-componente
```
Ou
```
ng g c nome-componente
```

---

## Como Funciona os componentes
![image](https://github.com/GabrielPilato/Funtec/assets/40001302/02cc9e20-876d-4b10-ade6-63a285400a06)
### Selector
Será o nome de HTML desse componente, podendo ser utilizado e puxado em diferentes páginas.

### TemplateUrl
Diz onde está o arquivo que será utilizado para apresentar esse componente, é nesse arquivo que será customizado a aparencia e a funcionalidade do componente

### StyleUrls
Um array de arquivos CSS para customizar o Template de HTML mencionado anteriormente

---

![image](https://github.com/GabrielPilato/Funtec/assets/40001302/ddf5f694-e0f6-4b07-8b7b-bd4fc5de094d) ![image](https://github.com/GabrielPilato/Funtec/assets/40001302/c530ab3d-9bd3-4f8d-befd-1c4d1bda8ba9)

---

### FormControlName e ngModel
Para melhor controle de formularios mais complexos, recebendo e enviando valores, ngModel é para formulários mais simples

### Buscando API's
```
ng g s nome-servico
```
