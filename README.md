🎯 Sistema de Recomendação Inteligente de Oportunidades Profissionais para o Mercado de Tecnologia

Projeto desenvolvido para a disciplina de Projeto Aplicado III - Curso de Ciência de Dados da Universidade Presbiteriana Mackenzie

👥 Integrantes da Equipe

Daniel dos Santos da Silva (RA: 10720767)

Enzo Ferroni (RA: 10417100)

Vinícius de Souza Sabiá (RA: 10721475)

📌 Objetivo do Projeto

O objetivo principal deste projeto é investigar a ineficiência no cruzamento (match) entre os perfis de profissionais de tecnologia (suas habilidades e senioridade) e os requisitos exigidos pelas vagas de emprego.

Para resolver isso, desenvolvemos um Sistema de Recomendação baseado em Conteúdo (Content-Based Filtering) utilizando algoritmos de Processamento de Linguagem Natural (TF-IDF com n-gramas) e Similaridade de Cosseno. O sistema atua de forma inteligente e escalável para sugerir oportunidades hiperpersonalizadas ao candidato, reduzindo ruídos e promovendo a inclusão produtiva no mercado de tecnologia (ODS 8).

📊 Metodologia e Resultados

O pipeline de treinamento do modelo foi constituído pelos seguintes passos:

Coleta e Limpeza: Tratamento de uma base original de 50.000 vagas. Aplicação de filtros rigorosos por Indústria (Software, IT), palavras-chave no Título e contagem de Habilidades. O dataset foi reduzido para 1.021 vagas altamente relevantes, removendo 98% do ruído.

Engenharia de Atributos: Criação de um perfil textual combinado (Título + Experiência + Habilidades) com conversão para lower case e remoção de stop words personalizadas do nicho de RH.

Vetorização: Implementação do TF-IDF com n-gramas (1,2), limitando a matriz matemática às 500 características mais valiosas.

Avaliação: O modelo foi validado quantitativamente usando a métrica Precisão@5, alcançando o melhor score ao combinar o título e bigramas. Qualitativamente, o modelo obteve sucesso em devolver o Top-5 de sugestões perfeitamente alinhadas com as hard skills do candidato simulado (ex: "Python, Machine Learning, SQL").

🔗 Links

💾 Base de Dados (Kaggle): [AI-Powered Job Recommendations](https://www.kaggle.com/datasets/samayashar/ai-powered-job-recommendations/data)

📄 Documentação Completa: [Leia o PDF na pasta docs/](docs/ProjetoAplicadoIII.pdf)

🎬 Apresentação do Projeto: [LINK YOUTUBE]
