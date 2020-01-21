# Docker Compose Nifi com LDAP

### Instalação

1. Pegar a ultima versão do pacote:
```sh
git clone https://github.com/WelAndrade/nifi.git
```
2. Incluir os certificados no diretorio certs.(Modificar as senhas no compose se necessário)
3. Configurar
- INITIAL_ADMIN_IDENTITY=' ' #Logon no LDAP do usuário que irá utilizar o ambiente
- LDAP_MANAGER_DN=' ' #Usuário com permissão de Leitura no LDAP
- LDAP_MANAGER_PASSWORD=' ' #Senha do usuário
- LDAP_USER_SEARCH_BASE=' ' # Base de pesquisa do LDAP
- LDAP_URL=' ' #Endereço do Servidor LDAP

4. Rodar:
```sh
docker-compose up
```
