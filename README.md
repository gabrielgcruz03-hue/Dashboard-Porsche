# Dashboard-Porsche
Dashboard interativa de vendas da Porsche, criada a partir de dados de transações reais. Permite explorar modelos mais vendidos, métodos de pagamento, status de entrega e distribuição geográfica. Publicada via GitHub Pages como evidência prática de análise de dados com IA.

Este projeto apresenta uma dashboard interativa construída a partir de uma base de dados de vendas de veículos Porsche.   

---

## 🔎 Perguntas de negócio escolhidas

As principais perguntas que guiaram a construção da dashboard foram:

1. **Quais modelos da Porsche mais vendem por ano?**  
   → Importante para identificar tendências de mercado e preferências dos clientes.

2. **Quais métodos de pagamento são mais utilizados?**  
   → Relevante para entender o comportamento financeiro dos compradores.

3. **Qual o status de entrega dos veículos vendidos?**  
   → Ajuda a monitorar logística e satisfação do cliente.

4. **Distribuição geográfica das vendas por estado/cidade.**  
   → Essencial para direcionar campanhas de marketing regional.

---

## 🧩 Prompt utilizado para gerar a dashboard

**Versão inicial do prompt:**
utilizando o recurso de canvas, renderize uma dashboard em html ao lado # Filtros modelo da porsche, model year, city e paymethod . # perguntas de negocios e kpis quais os principais modelos de carro vendidos por cidade, qual o ano de modelo de carro mais saiu em um periodo , quero um site de carros populares de vendas com base nos dados em cada cidade, sobre o ui/ux , se baseie no site da porsche brasil : https://www.porsche.com/brazil/pt/ . tenha um ar de elegante e refinado

**Versão final (ajustada):**
Filtre modelos de porsche, model year e city . perguntas de negocios e kpis são Quais os principais modelos de carros vendidos por cidade, Qual o ano do modelo do carro mais saiu em ano


As mudanças foram feitas para deixar o prompt mais **específico**, garantindo que a IA gerasse visualizações úteis e alinhadas às perguntas de negócio.

---


## 🛠️ Tratamento da base de dados

Antes de enviar a base para a IA, foram aplicados os seguintes ajustes:

- **Correção de datas inválidas**: várias linhas tinham `INVALID` em `SaleDateSanitized`.  
- **Normalização de nomes**: padronização de maiúsculas/minúsculas em `Sales Person`.  
- **Remoção de inconsistências**: alguns registros tinham valores decimais em `Sales Price` (ex.: `153200.5`), que foram arredondados.  
- **Validação de status de entrega**: padronização de categorias (`Delivered`, `Pending`, `Cancelled`, etc.).

---

## 🤖 Ferramentas utilizadas

- **ChatGPT com Canvas** para geração inicial da dashboard. 


---

## 📸 Evidências

### Print da tela
*(<img width="1886" height="950" alt="image" src="https://github.com/user-attachments/assets/db2c3731-e20c-4e25-9c5d-d6c2ccd32c8f" />)*
*(<img width="1864" height="845" alt="image" src="https://github.com/user-attachments/assets/17a34729-763d-4e54-a675-1e5a16f378d9" />)*
*(<img width="1832" height="846" alt="image" src="https://github.com/user-attachments/assets/08342241-b93d-4486-8462-295186d299c1" />)*



### Exemplo de filtro aplicado
- Filtro: **Modelo = 911 Turbo S**  
- Resultado: mostra apenas vendas relacionadas ao modelo 911 Turbo S, com gráficos atualizados dinamicamente.

---

## 🚀 Como rodar localmente

1. Clone este repositório:  git clone https://github.com/gabrielgcruz03-hue/Dashboard-Porsche/edit/main/README.md
