# Automação de Testes de API REST com Java + RestAssured 🚀

Projeto de testes automatizados de API utilizando **Java 11**, **RestAssured** e **JUnit 5**.  
Inclui testes funcionais (E2E), validações de respostas, boas práticas e relatórios detalhados.

## 📋 Funcionalidades

- ✅ Testes E2E completos de APIs REST
- ✅ Requisições HTTP (GET, POST, PUT, DELETE, PATCH)
- ✅ Validações avançadas de status code, headers e corpo JSON
- ✅ Testes parametrizados e organizados por funcionalidade
- ✅ Relatórios HTML claros e profissionais
- ✅ Configuração via variáveis de ambiente
- ✅ Código bem comentado e documentado para iniciantes
- ✅ Boas práticas de automação de testes

## 🛠️ Tecnologias Utilizadas

| Tecnologia       | Versão      |
|------------------|-------------|
| Java             | 11          |
| Maven            | 3.9.9       |
| RestAssured      | 4.4.0       |
| JUnit 5          | 5.10+       |
| IntelliJ IDEA    | Community   |
| Postman          | (validação manual) |

---

## 🚀 Instalação

```bash
# 1. Clone o repositório
git clone https://github.com/SEU_USUARIO/automacao-testes-api-restassured-java.git

# 2. Entre na pasta do projeto
cd automacao-testes-api-restassured-java

# 3. Instale as dependências
mvn clean install
```

## ⚙️ Configuração

**Crie um arquivo src/test/resources/config.properties ou use variáveis de ambiente:**
```bash
# config.properties
base.url=http://api.exemplo.com
username=seu_usuario
password=sua_senha
token=seu_token_aqui
```

**Dica: Nunca commite credenciais reais no Git!**

## 🧪 Executando os Testes

### 📊 Testes com Relatórios HTML
 ```bash
# Todos os testes + relatório
mvn test

# Apenas testes de uma funcionalidade específica
mvn test -Dtest=UsuarioTest
mvn test -Dtest=PedidoTest
```

### 🔍 Testes no Terminal
 ```bash
# Executar todos os testes
mvn test

# Executar apenas uma classe de teste
mvn test -Dtest=NomeDaClasseTest

# Executar um método específico
mvn test -Dtest=NomeDaClasseTest#nomeDoMetodo
```

## 📁 Estrutura do Projeto
```
automacao-testes-api-restassured-java/
├── src/
│   └── test/
│       └── java/
│           └── com/
│               └── seuusuario/
│                   ├── base/              # Configuração base (TestBase.java)
│                   ├── tests/             # Testes organizados
│                   │   ├── usuario/       # Ex: UsuarioTest.java
│                   │   ├── pedido/        # Ex: PedidoTest.java
│                   │   └── auth/          # Ex: AuthTest.java
│                   ├── utils/             # Helpers e builders
│                   ├── models/            # Classes de request/response
│                   └── schemas/           # Validações JSON Schema (opcional)
├── src/test/resources/
│   ├── config.properties
│   └── schemas/                           # JSON Schemas
├── pom.xml
├── README.md
├── .gitignore
└── target/surefire-reports/               # Relatórios gerados
```

## 🎯 Funcionalidades Testadas

### 🔄 Testes Funcionais E2E (End-to-end)

- ✅ Autenticação e geração de tokens
- ✅ CRUD completo (Criar, Consultar, Atualizar, Deletar)
- ✅ Validação de fluxos completos da API
- ✅ Testes com dados randômicos

### 📋 Validações

- Status codes esperados
- Estrutura e valores do JSON
- Campos obrigatórios e opcionais
- Performance básica (tempo de resposta)

## 📊 Scripts Maven Disponíveis

Adicione esses scripts no **pom.xml**:

| Comando       | Descrição      |
|------------------|-------------|
| mvn test         | Executa todos os testes |
| mvn test -Dtest=XXX | Executa testes específicos|
| mvn clean test     | Limpa e executa|


## 🚨 Solução de Problemas

### ☢️ Erro de dependências / classes vermelhas no IntelliJ

- Maven → Reload project
- File → Invalidate Caches → Invalidate and Restart

### Problemas com Java 17/21/25

- Use ♨️ ***Java 11*** (versão mais estável com RestAssured 4.4.0)

### ⚠️ Testes falhando por token

- Verifique o arquivo config.properties
- Rode primeiro o teste de autenticação

## 🔒 Segurança

- ❌ Nunca commite senhas, tokens ou dados sensíveis
- ✅ Use config.properties + .gitignore
- ✅ Adicione .env e target/ no .gitignore


## 🤝 Como Contribuir

1. Faça um Fork do projeto
2. Crie uma branch: git checkout -b feature/nova-funcionalidade
3. Commit: git commit -m 'feat: adiciona teste de X'
4. Push: git push origin feature/nova-funcionalidade
5. Abra um Pull Request

## 👤 Autora
**Janaína Mayara Valério** 💡 Estudante de Automação de Testes | 🥰 Apaixonada por Java & Qualidade de Software 💜

"Continue praticando. Programar é como dirigir: no começo parece difícil, mas com prática tudo se torna natural."
— Flávio D.

- E-mail: jm.janainamayara@hotmail.com
- GitHub: [@janaina-valerio](https://github.com/janaina-valerio)

  
⭐ **Deixe uma estrela se este projeto te ajudou! 💜**
