# App

GymPass style app api.

## RFs (Requisitos funcionais)

- [ ] Deve ser possível se cadastrar;
- [ ] Deve ser possível se autenticar;
- [ ] Deve ser possível obter o perfil de um usuário logado;
- [ ] Deve ser possível obter o número de check-ins realizdos pelo usuário logado;
- [ ] Deve ser possível o usuário obter seu histórico de check-ins;
- [ ] Deve ser possível o usuário buscar academias próximas;
- [ ] Deve ser possível o usuário buscar academias pelo nome;
- [ ] Deve ser possível o usuário realizar check-in em uma academia;
- [ ] Deve ser possível validar o check-in de um usuário;
- [ ] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócio)

- [ ] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [ ] O usuário não pode fazer 2 check-ins no mesmo dia;
- [ ] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [ ] O check-in só pode ser validado até 20 minutos após criado;
- [ ] O check-in só pode ser validado por administradores;
- [ ] A academia só pode ser cadastrada por administradores;

## RFs (Requisitos não-funcionais)

- [ ] A senha do usuário precisa estar criptografada;
- [ ] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [ ] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [ ] O usuário deve ser identificado por um JWT (JSON Web Token);

## Configurações do projeto

### Dependências de Desenvolvimento

```sh
# Adicionar typescript e seus tipos.
  npm install typescript @types/node tsx tsup -D
```

```sh
# Adicionar tsx para converter o código ts para js automaticamente e rodar o código em desenvolvimento.
  npm install tsx -D
```

```sh
# Adicionar tsup biblioteca para fazer o build da aplicação convertendo de ts para js para produção.
  npm install tsup -D
```

## Dependências de produção

```sh
# Adicionar tsc --init para criar o arquivo de configuração typescript.
  npx tsc --init
```

```sh
# Adicionar fastify para criar nosso servidor.
  npm install fastify
```

```sh
# Adicionar dotenv para carregar as variáveis de ambiente para o Node.js e assim temos acesso a elas.
  npm install dotenv
```

```sh
# Adicionar zod para fazer validações.
  npm install zod
```
