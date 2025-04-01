# 📊 Análise de Dados do iFood

## Descrição do Projeto
Este projeto tem como objetivo analisar dados relacionados ao iFood, focando na distribuição de restaurantes, avaliações e taxas de entrega por região do Brasil. Utilizando ferramentas como Pandas e PySpark, o estudo busca extrair insights relevantes sobre o funcionamento da plataforma.

## Tecnologias Utilizadas
- **Python 3.12**
- **Pandas**
- **PySpark**
- **Jupyter Notebook**

## Etapas da Análise
1. **Importação de Bibliotecas e Arquivos**  
   - Carregamento de bibliotecas como `pandas` e `pyspark`.
   - Leitura dos dados para um DataFrame.

2. **Verificação e Tratamento dos Dados**  
   - Testes para garantir que os dados foram carregados corretamente.
   - Criação da coluna "região" com base no estado.
   - Renomeação de colunas para melhor legibilidade.

3. **Análise Exploratória**  
   - Cálculo da média da taxa de entrega por região.
   - Análise da média das avaliações dos restaurantes em cada região.
   - Análises da quantidade de restaurante custo beneficio por região.
   - Analise das Principais Categorias de restaurante de cada região por quantidade e por avaliação.
   - Crescimento de restaurantes entre 2020 e 2021.

## Como Executar o Projeto
1. Certifique-se de ter o Python 3.12 instalado.
2. Instale as dependências necessárias utilizando:
   ```bash
   pip install pandas pyspark
   ```
3. Execute o notebook utilizando um ambiente compatível, como Jupyter Notebook ou Google Colab.

# Resultados e Insights
## 🔹 Análise da Média da Taxa de Entrega por Região  

### **Insights sobre as Taxas de Entrega**  

### 🏆 Centro-Oeste tem a maior média de taxa de entrega (8.18)  
- Essa região apresenta a maior taxa média entre todas.  
- Isso pode ser explicado por distâncias maiores entre os pontos de entrega devido à menor densidade populacional, além da possível menor quantidade de entregadores disponíveis, o que encarece o serviço.  

### 📈 Nordeste também tem taxas elevadas (8.02)  
- A média do Nordeste é a segunda mais alta, sugerindo desafios logísticos semelhantes aos do Centro-Oeste.  
- O custo do transporte e a infraestrutura podem ser fatores que impactam diretamente o valor cobrado pelas entregas.  

### 📉 Sul, Sudeste e Norte têm taxas mais baixas  
- **Sudeste (7.72), Sul (7.74) e Norte (7.70)** possuem as menores médias de taxas de entrega.  
- No caso do **Sudeste e Sul**, isso pode estar relacionado à maior quantidade de restaurantes cadastrados e à alta demanda de pedidos, tornando as entregas mais frequentes e reduzindo os custos operacionais.  
- No **Norte**, uma possível explicação é que o iFood pode estar aplicando estratégias promocionais para atrair mais clientes e expandir a plataforma na região.  



## 🔹 Análise da Média das Avaliações dos Restaurantes em 2020 e 2021  

### **Insights sobre as Avaliações**  

### 🔄 **Estabilidade nas Avaliações do Nordeste**  
- A média do Nordeste permaneceu inalterada (**4.46**), indicando que a percepção dos clientes sobre os restaurantes não mudou significativamente.  
- Isso sugere que o serviço e a qualidade dos restaurantes se mantiveram constantes.  

### 📈 **Pequena Melhora no Norte**  
- A média do Norte subiu de **4.41 para 4.44**, um leve aumento.  
- Isso pode indicar melhorias na qualidade do atendimento ou nos serviços de entrega.  

### 📉 **Leve Queda no Centro-Oeste e Sudeste**  
- No **Centro-Oeste**, a média caiu de **4.50 para 4.49**, e no **Sudeste**, de **4.53 para 4.52**.  
- Essas quedas são pequenas, mas podem indicar um aumento na exigência dos clientes ou possíveis desafios logísticos que impactaram a experiência.  

### 🥇 **Sul Continua sendo a Região com Melhor Avaliação, mas Caiu um Pouco**  
- O **Sul ainda tem a maior média de avaliação**, mas caiu de **4.59 para 4.55**.  
- Apesar da leve queda, os restaurantes da região continuam sendo os melhores avaliados.  



## 🔹 Análise da Quantidade de Restaurantes com Custo-Benefício por Região  

### **Insights sobre Restaurantes com Custo-Benefício**  

### 🏆 **Sudeste domina em quantidade de restaurantes com custo-benefício**  
- A região Sudeste tem **1.371 restaurantes**, muito acima das demais regiões.  
- Isso pode ser explicado pela maior quantidade de restaurantes cadastrados no iFood e pela alta concorrência, incentivando preços mais competitivos.  

### 🥈 **Nordeste ocupa o segundo lugar, mas com um número bem menor**  
- Com **308 restaurantes**, o Nordeste ainda se destaca, mas tem uma quantidade muito inferior ao Sudeste.  
- Isso pode indicar que a concorrência entre restaurantes é menor ou que o conceito de custo-benefício é diferente na região.  

### 🥉 **Sul segue próximo do Nordeste**  
- Com **292 restaurantes**, o Sul tem um número parecido com o Nordeste, sugerindo que a estratégia de preços acessíveis é relevante nessas regiões.  

### 📉 **Centro-Oeste e Norte possuem a menor quantidade**  
- O **Centro-Oeste (81 restaurantes)** e o **Norte (71 restaurantes)** têm a menor oferta de restaurantes com custo-benefício.  
- Isso pode estar relacionado a uma menor diversidade gastronômica, menor adesão ao iFood ou custos operacionais mais altos para os restaurantes dessas regiões.  



## 🔹 Análise das Principais Categorias de Restaurantes de Cada Região  

### **Insights sobre as Categorias de Restaurantes**  

### 🍔 **1. Lanches dominam em todas as regiões**  
- A categoria **"Lanches"** é a mais comum e a mais bem avaliada em todas as regiões do Brasil.  
- Isso indica que hambúrgueres, sanduíches e fast food são extremamente populares e bem aceitos pelos consumidores do iFood.  
- Além disso, a praticidade desse tipo de comida pode contribuir para sua alta demanda.  

### 🍛 **2. Comida Brasileira está sempre no Top 2**  
- A categoria **"Brasileira"** aparece como a segunda mais comum e a segunda mais bem avaliada em todas as regiões.  
- Isso mostra que pratos tradicionais ainda são muito valorizados pelos consumidores, independentemente da localização.  
- A forte presença dessa categoria sugere que os clientes procuram conforto e familiaridade na comida.  

### 🍕 **3. Pizza é popular, mas perde espaço para doces em algumas regiões**  
- No **Nordeste, Norte e Sul**, a categoria **"Pizza"** aparece como a terceira mais popular e bem avaliada.  
- No **Centro-Oeste e Sudeste**, porém, **"Doces & Bolos"** supera a pizza em quantidade de restaurantes.  
- Isso pode indicar uma demanda maior por sobremesas e confeitarias nessas regiões, possivelmente impulsionada por cafeterias e padarias.  

### 🌎 **4. Sudeste tem um número muito maior de restaurantes cadastrados**  
- A diferença na quantidade de restaurantes é impressionante: o **Sudeste tem 60.764 restaurantes de lanches**, enquanto o segundo colocado (**Sul**) tem **16.353**.  
- Isso reflete a densidade populacional maior e a competitividade da região, o que pode oferecer mais opções de escolha e preços melhores para os consumidores.  

### 📊 **5. A relação entre quantidade e qualidade**  
- Nem sempre as categorias mais numerosas são as mais bem avaliadas.  
- A porcentagem de restaurantes bem avaliados dentro de cada categoria pode variar, mostrando que a concorrência pode impactar a qualidade percebida pelos clientes.  



## 🔹 Crescimento de Restaurantes entre 2020 e 2021  

### **Insights sobre o Crescimento de Restaurantes no iFood (2020-2021)**  

### 📈 **1. Crescimento expressivo de 12.08%**  
- Um aumento de **12.08%** no número de restaurantes cadastrados em um único ano mostra que o iFood continuou expandindo sua base de estabelecimentos.  
- Isso pode ter sido impulsionado pelo crescimento do delivery como hábito permanente dos consumidores, especialmente após o impacto da pandemia em 2020.  

### 📊 **2. +37.277 novos restaurantes em um ano**  
- Esse volume de novos cadastros representa uma grande adesão de estabelecimentos ao delivery.  
- Pequenos e médios empreendedores podem ter migrado para o iFood como alternativa para manter ou expandir seus negócios.  

### 🌐 **3. Possível impacto da digitalização e da recuperação econômica**  
- Muitos restaurantes que não trabalhavam com delivery antes da pandemia podem ter aderido à plataforma para alcançar novos clientes.  
- A flexibilização das restrições em 2021 também pode ter incentivado a entrada de novos restaurantes no mercado.  


## 📊 Dashboard Interativo no Power BI  

O arquivo localizado no diretório `DashBoard_PowerBI` contém um **dashboard interativo** desenvolvido no **Power BI**, apresentando as análises realizadas neste projeto.  

Esse dashboard permite a visualização dinâmica dos dados, facilitando a interpretação dos insights extraídos.  




