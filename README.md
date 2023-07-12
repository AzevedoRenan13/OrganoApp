# Documentação da Aplicação
## Introdução
Esta é uma aplicação React que apresenta um formulário para cadastrar colaboradores em diferentes times. Os times são exibidos em cards com suas respectivas cores primárias e secundárias. Cada colaborador cadastrado é exibido no time correspondente.

## Componentes
A aplicação é composta pelos seguintes componentes:

## App
O componente App é o componente principal que renderiza toda a aplicação. Ele possui o estado colaboradores que armazena a lista de colaboradores cadastrados. O componente também define a função aoNovoColaboradorAdicionado que é responsável por adicionar um novo colaborador à lista.

## Estado
 colaboradores: uma lista de objetos representando os colaboradores cadastrados. Cada objeto possui as propriedades nome (string), email (string) e time (string) representando o nome, e-mail e time do colaborador, respectivamente.
### Banner
O componente Banner exibe um banner na parte superior da página.

## Formulario
O componente Formulario exibe um formulário onde os usuários podem cadastrar novos colaboradores. Ele recebe a lista de nomes dos times disponíveis como prop times e a função aoColaboradorCadastrado como prop aoColaboradorCadastrado, que é chamada quando um novo colaborador é cadastrado.

## Props
times: uma lista de nomes de times disponíveis para seleção.
aoColaboradorCadastrado: uma função que é chamada quando um novo colaborador é cadastrado. Recebe o objeto colaborador como argumento, contendo as propriedades nome, email e time do colaborador cadastrado.
## Time
O componente Time exibe um card representando um time. Ele recebe as informações do time, incluindo o nome, cores primária e secundária, e a lista de colaboradores pertencentes a esse time.

## Props
nome: o nome do time.
corPrimaria: a cor primária do time, representada como uma string hexadecimal.
corSecundaria: a cor secundária do time, representada como uma string hexadecimal.
colaboradores: uma lista de objetos representando os colaboradores pertencentes a esse time. Cada objeto possui as propriedades nome, email e time representando o nome, e-mail e time do colaborador, respectivamente.
# Fluxo da Aplicação
## A aplicação segue o seguinte fluxo:

O componente App é renderizado e exibe o componente Banner no topo da página.
Em seguida, o componente Formulario é renderizado. Ele recebe a lista de nomes dos times disponíveis como prop times e a função aoColaboradorCadastrado como prop aoColaboradorCadastrado.
Quando um usuário preenche e envia o formulário, a função aoColaboradorCadastrado é chamada no componente Formulario. Essa função adiciona o novo colaborador à lista de colaboradores no estado colaboradores do componente App.
Após o cadastro de um novo colaborador, o componente App renderiza os componentes Time para cada time na lista times. Ele passa as informações do time e a lista filtrada de colaboradores pertencentes a esse time como props para cada componente Time.
Cada componente Time exibe as informações do time, incluindo seu nome e cores primária e secundária, bem como a lista de colaboradores pertencentes a esse time.
Considerações Finais
Esta é uma documentação básica da aplicação, fornecendo informações sobre seus componentes, props e fluxo de funcionamento. Caso haja necessidade de informações mais detalhadas ou alguma funcionalidade específica não esteja documentada, por favor, forneça mais detalhes para que eu possa ajudar de forma mais precisa.
