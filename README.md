# tri2-ia22-autenticacao-20223138883

## O que é autenticação de dados(single server)?

### O Que É?

Autenticação em um único servidor é o processo de verificar se um usuário é quem diz ser, usando apenas um servidor para gerenciar todo o processo.

### Como Funciona?

Login: O usuário envia seu nome de usuário e senha para o servidor.
Verificação: O servidor confere se essas credenciais estão corretas.
Sessão: Se estiver tudo certo, o servidor cria uma "sessão" para o usuário, que é como uma forma de lembrar que ele está autenticado.
Acesso: O usuário pode acessar recursos protegidos enquanto a sessão estiver ativa.
Logout: O usuário pode se desconectar, e o servidor encerra a sessão

## Autenticação VS Autorização

Autenticação
O Que É? Verifica quem você é.
Como Funciona? Você fornece suas credenciais (como nome de usuário e senha), e o sistema confirma sua identidade.
Exemplo: Entrar na sua conta de e-mail com seu nome e senha.

Autorização
O Que É? Define o que você pode fazer.
Como Funciona? Depois de verificar sua identidade, o sistema decide quais recursos e ações você tem permissão para acessar ou realizar.
Exemplo: Mesmo que você tenha entrado na sua conta de e-mail, apenas alguns usuários podem acessar configurações administrativas

resumindo a autenticação confirma quem vc é, já a autorização define suas permissões

Autenticação com Token (JWT)

O Que É JWT?
JWT (JSON Web Token) é uma maneira de garantir que um usuário está autenticado e permitir acesso a recursos de forma segura.

(alguns passos)

Login:

O usuário envia nome de usuário e senha para o servidor.

Gerar Token:

Se as credenciais estiverem corretas, o servidor cria um JWT.
O JWT contém informações sobre o usuário e uma assinatura para garantir que não foi alterado.

Enviar Token:

O servidor envia o JWT de volta para o usuário.

Armazenar Token:

O usuário armazena o JWT no navegador (em cookies ou local storage).

Requisições Futuras:

Para acessar áreas protegidas, o usuário envia o JWT junto com a solicitação.
O servidor verifica o JWT para confirmar a identidade e autorizar o acesso.

Estrutura do JWT

Cabeçalho: Define o tipo de token e o algoritmo de assinatura.
Payload: Contém dados sobre o usuário, como ID e permissões.
Assinatura: Garante que o token não foi alterado.

Projeto (Objeto de Estudos)

alguns aspectos devem ser considerados na criação do projeto como:

Escopo: Definindo claramente como o projeto será realizado.
Arquitetura: Planejar como o sistema de autenticação e autorização.
Segurança: Criptografias e sistemas de segurança muito fortes devem ser criados pois terão muitos dados a ser utilizados que nescessitam de segurança.
Interface do usuário: Criando uma parte para registro do usuário como login e senha.
Testes e validação: Criar testes e validações para que o não haja erros na entrega.
Documentação: Documente o fluxo das autenticações, formato dos tokens entre outros.



