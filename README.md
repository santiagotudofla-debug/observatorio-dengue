# 🧬 Observatório Dinâmico de Arboviroses e Saúde Pública
**Painel Executivo de Vigilância Epidemiológica com Integração em Tempo Real**

[![Streamlit](https://img.shields.io/badge/Deploy-Streamlit_Cloud-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](URL_DO_SEU_APP_AQUI)
[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![Data Science](https://img.shields.io/badge/Data_Science-Public_Health-2dc653?style=for-the-badge)]()

## 📌 Visão Geral
Este projeto é um **Data Product (Produto de Dados)** focado em inteligência epidemiológica para o combate à Dengue, Zika e Chikungunya. Desenvolvido para atuar como uma "Sala de Situação" (War Room), o sistema consome dados abertos em tempo real para transformar estatísticas de saúde em diretrizes de ação executiva.

A plataforma foi projetada para ter **escalabilidade nacional**, permitindo o monitoramento de mais de 5.570 municípios brasileiros através de geoprocessamento e modelagem preditiva.

---

## 🏛️ O Grande Diferencial: Economia da Saúde para Gestores Públicos
Enquanto a maioria dos painéis epidemiológicos foca apenas na volumetria clínica (número de casos), este projeto introduz um módulo inédito de **Economia da Saúde (Health Economics)**.

Este módulo foi criado especificamente para **Prefeitos e Secretários de Saúde**, traduzindo a sobrecarga hospitalar em **Balanço Financeiro (Custo Brasil da Dengue)**. 

**O que este módulo calcula:**
- 💸 **Drenagem Orçamentária:** Estimativa de gastos do tesouro municipal segmentada por gravidade (Consultas Ambulatoriais vs. Leitos de Observação vs. Internações em UTI).
- 📉 **Impacto no PIB Local:** Cálculo de absenteísmo (dias de trabalho perdidos) e o rombo gerado na economia produtiva da cidade.
- 💡 **ROI da Prevenção:** Comprovação matemática de que o custo de **uma única internação grave** financia mais de 120 intervenções primárias (como visitas de agentes de endemias ou caminhões de fumacê).

---

## 📡 Fontes de Dados (Integração em Tempo Real)
Este projeto **não utiliza dados estáticos ou planilhas locais**. Ele é alimentado diretamente por APIs governamentais e de pesquisa de alto nível:

1. **InfoDengue (Fiocruz / FGV):** Alimentação do motor de *Nowcasting* (previsão em tempo real), fornecendo estimativas de casos, Taxa de Transmissibilidade (Rt) e fatores climáticos oficiais do Ministério da Saúde.
2. **API IBGE:** Consumo do geocódigo e da população atualizada do município pesquisado para o cálculo preciso da incidência por 100 mil habitantes.
3. **OpenStreetMap (Overpass API):** Varredura via satélite que mapeia as Unidades de Pronto Atendimento (UPAs) e hospitais reais em um raio de 15km da cidade escolhida, gerando um ranking autônomo de pressão hospitalar.

---

## 🛠️ Funcionalidades e Módulos Analíticos

- **🛡️ Centro de Comando (War Room):** Simulador tático (What-If Analysis) que permite prever o achatamento da curva caso medidas de limpeza sejam adotadas.
- **📈 Série Temporal & API:** Comparação visual entre as notificações físicas (sujeitas a atrasos de digitação no SINAN) e o modelo de Inteligência Artificial do InfoDengue.
- **🌦️ Correlação Climática:** Gráficos que cruzam a temperatura média com a explosão de casos e a evolução do limiar crítico do Rt.
- **🔮 Forecast Preditivo:** Algoritmo de extrapolação que avalia a inclinação da curva e emite alertas (ALTA ou QUEDA) para as próximas 4 semanas.
- **🗺️ Mapeamento Geoespacial:** Mapas de calor (Heatmaps) dinâmicos gerados via Folium para otimização de rotas de controle de Zoonoses.
- **📥 Extração Executiva:** Gerador de relatórios acoplado. Com um clique, o sistema fabrica um arquivo **PowerPoint (.pptx)** formatado com os achados da cidade para ser apresentado em reuniões de diretoria, além da extração de microdados em `.csv`.

---

## 🚀 Como Executar o Projeto Localmente

**1. Clone o repositório**
```bash
git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)
cd SEU_REPOSITORIO
