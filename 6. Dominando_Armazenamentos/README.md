# Guia Completo de Armazenamento no Azure | Migração e Gerenciamento de Dados

---

## 1. Acessar o Portal do Azure 

1. Acesse o https://portal.azure.com/ e faça login com suas credenciais.
2. No painel de navegação à esquerda, clique em **Criar um recurso**.

---

## 2. Criar e Configurar uma Conta de Armazenamento 

### Iniciar Criação

1. Na barra de pesquisa, digite **Conta de Armazenamento** e selecione **Criar**.
2. Preencha os detalhes básicos:
   - **Assinatura**: Escolha a assinatura desejada.
   - **Grupo de Recursos**: Selecione ou crie um novo.
   - **Nome da Conta**: Insira um nome único (3-24 caracteres, letras minúsculas e números).
   - **Região**: Selecione a região mais próxima dos usuários.
   - **Desempenho**: Escolha entre **Padrão** ou **Premium**.
   - **Tipo de Conta**: Opte por "Armazenamento General Purpose v2".
   - **Replicação**: Defina o tipo de replicação (LRS, GRS, ZRS).

### Configurações Avançadas

1. Ative a **transferência segura** para exigir HTTPS.
2. Habilite **Large file shares** para Azure Files.
3. Ative o **Hierarchical Namespace** para Azure Data Lake Storage Gen2.

### Configurações de Rede e Segurança

1. Configure o método de conexão: **Público** ou **Privado**.
2. Defina regras de **Firewall e Redes Virtuais**.
3. Habilite a **Criptografia no Armazenamento** para segurança em repouso.

### Finalização

1. Clique em **Revisar + criar** e depois em **Criar**.

---

## 3. Configurar o Armazenamento Blob 

1. Acesse **Serviços de Armazenamento** e selecione **Containers**.
2. Crie um novo container e defina o nível de acesso: **Privado** ou **Público**.
3. Carregue arquivos diretamente ou utilize o **Azure CLI** ou **Azure Storage Explorer**.

---

## 4. Criar um Compartilhamento de Arquivos 

1. Na Conta de Armazenamento, clique em **File Shares**.
2. Adicione um novo compartilhamento, defina o nome e o tamanho.
3. Monte o compartilhamento em uma VM ou servidor usando o protocolo SMB.

---

## 5. Utilizar o Armazenamento de Tabelas 

1. No painel da Conta de Armazenamento, clique em **Tabelas**.
2. Adicione uma nova tabela e gerencie os dados com o **Azure SDK** ou **API REST**.

---

## 6. Gerenciar o Armazenamento de Filas 

1. Na Conta de Armazenamento, clique em **Filas**.
2. Crie uma nova fila e configure permissões de acesso.
3. Use a **API REST** ou o **SDK do Azure** para enviar e receber mensagens.

---

## 7. Migrar Dados para o Azure

1. Criar um Projeto de Migração:
   - Use ferramentas como o Azure Migrate para facilitar a migração.
2. Instalar o AzCopy:
   - Baixe do [site oficial](https://docs.microsoft.com/azure/storage/common/storage-use-azcopy-v10).
3. Autenticar com o Azure:
   - Siga as instruções para autenticação segura.

---

## 8. Monitoramento e Alertas 

1. Utilize o **Azure Monitor** para acompanhar o uso do armazenamento.
2. Configure **alertas** para notificações sobre capacidade e falhas.

## 9. Gerenciar Backups e Replicação

1. Configure o **Azure Backup** para recuperação de dados.
2. Habilite a **Geo-Redundância** para garantir segurança em desastres.
