# 🔍 Organização e Análise de Dados de Canais Bitflip  

Este notebook tem como objetivo processar e organizar os dados extraídos de um arquivo `.TXT`, contendo informações sobre a fidelidade inicial, requisição e a respectiva porcentagem de sucesso. O resultado final é uma planilha do Excel formatada, facilitando a análise dos dados.  

## 📌 Passos do Algoritmo  

### 1️⃣ Definição das Fidelidades  
- Criamos listas para representar os valores de **fidelidade inicial** (de `0.50` a `1.00`) e de **fidelidade de requisição** (de `0.51` a `1.00`).  
- Geramos um **DataFrame (`pandas`)**, preenchido inicialmente com `"x"` para indicar onde a requisição é menor ou igual à fidelidade inicial.  

### 2️⃣ Leitura do Arquivo de Dados  
- O arquivo de texto é lido linha por linha.  
- Expressões regulares (`re`) são usadas para identificar e extrair os valores de:
  - **Fidelidade inicial**  
  - **Requisição**  
  - **Porcentagem de sucesso**  

### 3️⃣ Processamento e Organização dos Dados  
- Um dicionário armazena os valores extraídos, associando cada combinação de fidelidade inicial e requisição à sua respectiva taxa de sucesso.  
- O **DataFrame é atualizado** com as porcentagens de sucesso, substituindo os valores `"x"` pelos dados extraídos.  

### 4️⃣ Geração da Planilha Excel  
- Os dados processados são exportados para um arquivo `.xlsx`, nomeado **"Valores de 0.5 até 1 Canais Bitflip.xlsx"**, para facilitar a análise.  

## 📊 Benefícios do Algoritmo  

✔ **Automação da organização de dados**, reduzindo erros manuais.  
✔ **Facilidade na análise**, com as porcentagens de sucesso formatadas diretamente na planilha.  
✔ **Eficiência no processamento**, manipulando milhares de registros rapidamente.  

---

🚀 **Com esse algoritmo, foi possível processar e estruturar mais de 15 mil dados, distribuídos em três planilhas, cada uma contendo 2.400 registros!**
