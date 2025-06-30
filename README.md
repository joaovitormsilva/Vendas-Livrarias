# 📊 Análise de Vendas de uma Livraria com PySpark no Databricks

Este projeto realiza a análise de um arquivo de vendas de uma livraria utilizando **Apache Spark (PySpark)** no ambiente **Databricks Community Edition**.

---

## 🚀 Tecnologias Utilizadas

- **Python 3.5 (com PySpark)**  
- **Apache Spark**: Processamento distribuído de dados em larga escala  
- **Databricks Community Edition**: Plataforma gratuita com notebooks colaborativos  
- **Unittest**: Framework de testes unitários do Python  

---

## ⚙️ Instalação e Configuração

### 1. Criar Conta no Databricks Community Edition

- Acesse: [Databricks Community](https://community.cloud.databricks.com/)
- Crie uma conta gratuita

### 2. Importar os Arquivos

- Vá até: `Workspace > [seu usuário] > Create > Folder`
- Crie uma pasta chamada **`vendas_livraria`**
- Dentro dela, importe os seguintes arquivos:
  - `vendas_livraria.ipynb`
  - (Opcional) `test_vendas_livraria.py.ipynb` – caso deseje rodar os testes unitários

### 3. Criar a Tabela no Databricks

- Abra o notebook `vendas_livraria`
- Vá em `File > Add Data > Create or Modify Table`
- Importe o arquivo `vendas_livros.csv`
- Aguarde o preview da tabela e clique em **"Create Table"**

---

## ▶️ Como Executar o Projeto

Abra o notebook `vendas_livraria.ipynb` e:

1. Altere o caminho do arquivo, se necessário  
   Ex: `workspace.default.vendas_livros`
2. Execute todas as células para:
   - Carregar os dados  
   - Rodar os testes de qualidade da tabela  
   - Criar a tabela `resumo_vendas_diarias`  
   - Descobrir o autor mais vendido  
   - Identificar a data campeã de vendas  

---

## 🧪 Executando os Testes

- Crie um notebook separado com o conteúdo de `test_vendas_livraria.py.ipynb`
- Execute o notebook
- Os testes verificarão:
  - Leitura correta da tabela  
  - Schema correto  
  - Mínimo de 10 datas distintas  
  - Ausência de datas futuras  
  - Se existem IDs negativos  

---

## 🛠️ Justificativas Técnicas

- **Apache Spark com PySpark**: Escolhido pela escalabilidade e eficiência para processar grandes volumes de dados  
- **Databricks Community Edition**: Permite desenvolvimento com Spark gratuitamente, com ambiente interativo e gerenciado  
- **Unittest**: Leve, robusto e integrado ao Python, facilita a validação e reprodutibilidade  
- **Arquitetura Medalhão**: Utilizada para organizar e validar dados em camadas, garantindo integridade e governança (ACID)

---

## 📝 Notas

Durante o desenvolvimento, busquei aplicar:

- Boas práticas de codificação com PySpark  
- Uma estrutura reutilizável e escalável  
- Testes unitários para validar transformações críticas

---

## 🔮 Melhorias Futuras

- Criar um pipeline de monitoramento contínuo com agendamento automático  
- Testar também as funções de transformação e as queries SQL de qualidade  

---

## 🙏 Obrigado!

Este projeto mostrou como o **Databricks Community Edition** pode ser uma excelente porta de entrada para trabalhar com **Spark** de forma prática e gratuita — ideal para quem está aprendendo ou prototipando soluções em larga escala.
