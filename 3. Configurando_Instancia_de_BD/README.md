# Configuração de um Banco de Dados SQL no Azure

## 1. Criando sua Conta no Azure 

Antes de iniciar, certifique-se de ter uma conta ativa no Azure. Se ainda não tiver, visite [portal.azure.com](https://portal.azure.com) para criar uma conta gratuita. Uma vez com a conta ativa, faça login no portal.

---

## 2. Acessando o Portal do Azure 

Após o login, acesse o https://portal.azure.com. No painel principal, utilize a barra de pesquisa no topo e digite **"SQL Database"**. Nos resultados, selecione a opção **"Banco de Dados SQL"** ou **"SQL Database"**. Em seguida, clique em **"Criar"** para iniciar o processo de configuração do banco de dados.

---

## 3. Preenchendo as Informações Básicas

- **Nome do Banco de Dados**: Escolha um nome único e fácil de lembrar para identificar seu banco de dados.
- **Assinatura**: Selecione a assinatura do Azure que deseja utilizar. Caso esteja testando, considere a opção gratuita, se disponível.
- **Grupo de Recursos**: Selecione um grupo de recursos já existente ou crie um novo. Os grupos de recursos ajudam a organizar seus recursos no Azure.
- **Servidor**: Você pode escolher um servidor existente ou criar um novo:
  - **Nome do Servidor**: Escolha um nome exclusivo para seu servidor SQL.
  - **Localização**: Selecione a região mais próxima para hospedar o servidor.
  - **Login de Administrador**: Insira um nome de usuário para o administrador do servidor.
  - **Senha**: Crie uma senha forte para o login do administrador.

---

## 4. Configurações de Plano de Serviço 

- **Camadas de Serviço**:
  - **Basic**: Ideal para bancos de dados pequenos e uso leve.
  - **Standard**: Equilibrado para cargas de trabalho moderadas.
  - **Premium**: Para bancos de dados críticos com altas exigências de desempenho.
  - **Hiperescala**: Para bancos de dados extremamente grandes que precisam de escalabilidade rápida.

---

## 5. Configurações de Rede 

- **Método de Conexão**:
  - **Ponto de Extremidade Público**: Permite conexões de fora do Azure (acesso via internet).
  - **Ponto de Extremidade Privado**: Restringe o acesso apenas à sua rede virtual no Azure.
  
- **Firewall do Servidor**: 
  - **Adicionar IP**: Clique em **"Adicionar meu IP atual"** para permitir que seu endereço IP tenha acesso ao banco de dados.
  - **Regras de Firewall**: Adicione outros IPs ou configure regras para permitir ou restringir o acesso conforme necessário.

---

## 6. Configurações de Segurança 

- **Autenticação do Azure Active Directory (AAD)**: Integre com o Azure AD para gerenciar quem pode acessar o banco de dados.
- **Azure Defender for SQL**: Habilite para detecção avançada de ameaças e proteção contra atividades suspeitas no banco de dados.
- **Auditoria e Monitoramento**: Ative auditoria para registrar o acesso ao banco de dados e acompanhar o uso e mudanças feitas nele.

---

## 7. Backup e Redundância de Dados 

- **Backup Geo-Redundante**: Habilite esta opção para garantir que backups do banco de dados sejam replicados em diferentes regiões geográficas. Isso oferece maior resiliência em casos de falhas regionais.
- **Redundância Local**: Para backups dentro da mesma região, garantindo recuperação em caso de falhas locais.

---

## 8. Revisar e Criar 

---

## 9. Conectando-se ao Banco de Dados 

1. Vá até **SQL Databases** no menu à esquerda do portal.
2. Selecione o banco de dados recém-criado.
3. No painel de visão geral, copie o **Nome do Servidor**.
4. Abra o SSMS ou Azure Data Studio e insira o **Nome do Servidor**, **Login de Administrador** e **Senha** que você configurou anteriormente.
5. Conecte-se ao banco de dados e comece a executar consultas, adicionar dados e explorar as funcionalidades do **Azure SQL Database**.

---

## 10. Você configurou com sucesso uma instância de banco de dados no Azure.
