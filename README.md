# Avaliacao do Pe Diabetico no PEC e-SUS APS

Projeto academico desenvolvido na disciplina de Analise de Sistemas e UML do Programa de Pos-Graduacao em Informatica em Saude (PPGINFOS) da Universidade Federal de Santa Catarina (UFSC).

## Objetivo do Projeto

Conceber a especificacao funcional, modelo de dados e prototipo de um formulario estruturado e interativo para avaliacao do pe diabetico, integrado ao Prontuario Eletronico do Cidadao (PEC e-SUS APS). O sistema implementa a classificacao automatica de risco segundo diretrizes clinicas internacionais (IWGDF 2023) e nacionais (PCDT DM2 2026), vinculando a realizacao do exame ao cumprimento da Boa Pratica F do indicador C4 da Atencao Primaria a Saude.

## Equipe e Papeis

* Damares Gaia: Analista de Requisitos e Normas
* Jennifer Tamara: Especialista de Dominio
* Karen Pinedo: Product Owner (PO) e UX
* Willy Smith: Analista Tecnico e Integracoes

## Metodologia de Desenvolvimento

O projeto segue as etapas do Processo de Desenvolvimento de Software Centrado no Usuario (UCD), fundamentado no livro da disciplina (Wazlawick et al., 2025):

1. Briefing: Alinhamento de escopo com o gestor, entrevista semiestruturada e primeira versao da Matriz CSD.
2. Imersao: Pesquisa secundaria (Desk Research) com mapeamento em radar (What's on your radar?), analise comparativa de cinco similares nacionais e internacionais (Benchmarking) e segunda versao da Matriz CSD.
3. Definicao e MVP: Criacao da persona primaria (Camila Andrade, enfermeira da Estrategia Saude da Familia), elaboracao do Mapa de Empatia e Canvas de Proposta de Valor, priorizacao de funcionalidades via tecnica MoSCoW e terceira versao da Matriz CSD.
4. Ideacao (Proxima Etapa): Mapeamento dos fluxos da consulta SOAP no PEC, geracao de alternativas visuais e wireframes de baixa fidelidade.
5. Prototipacao (Etapa Futura): Elaboracao de prototipo navegavel de alta fidelidade no Figma em conformidade com o Design System do e-SUS APS.
6. Validacao (Etapa Futura): Testes de usabilidade com profissionais de saude da Atencao Primaria, avaliacao de tempo de preenchimento e aplicacao da System Usability Scale (SUS).

## Estrutura do Repositorio

```text
mestrado-analise-de-sistemas/
│
├── index.html                   # Linha do tempo metodologica e portal do projeto
│
├── etapas/                      # Paginas web dedicadas a cada fase metodologica
│   ├── 01-briefing/             # Sintese do alinhamento com cliente e gestor
│   ├── 02-imersao/              # Desk research e visualizador What's on your radar?
│   ├── 03-definicao/            # Persona, Mapa de Empatia, MoSCoW e Matriz CSD 3
│   ├── 04-ideacao/              # Instrucoes e diretrizes da etapa de ideacao
│   ├── 05-prototipacao/         # Diretrizes de construcao do prototipo no Figma
│   └── 06-validacao/            # Protocolo de testes de usabilidade com usuarios
│
├── documentos/                  # Documentos tecnicos elaborados pela equipe
│   ├── 01-briefing/             # Registros de briefing (.docx)
│   ├── 02-imersao/              # Relatorios de entrevista, benchmark e slides (.docx / .pdf)
│   └── 03-definicao/            # Ficha da Persona Camila, MoSCoW e slides (.docx / .pdf)
│
└── referencias/                 # Biblioteca normativa e protocolos clinicos
    ├── normas-ms/               # Nota C4, PCDT DM2 2026, Manuais e Cadernos do MS
    ├── diretrizes-clinicas/     # Diretrizes IWGDF 2023 e Sociedade Brasileira de Diabetes
    └── disciplina/              # Livro-texto da disciplina e plano de ensino
```

## Nucleo do Produto (MVP - Must Have)

1. Formulario Estruturado: Campos clicaveis nos eixos de inspecao da pele, vascular (pulsos pedioso e tibial posterior) e sensibilidade protetora plantar.
2. Classificacao de Risco Sugerida: Calculo da categoria de 0 a 3 baseado no IWGDF 2023 / PCDT DM2 2026 pelo pior pe avaliado, com justificativa clinica visivel.
3. Decisao Clinica Humana: O profissional responsavel valida, confirma ou altera a categoria sugerida antes do encerramento do atendimento.
4. Faturamento do Indicador C4: Disparo automatico do procedimento SIGTAP 03.01.04.009-5 inserido no atendimento individual ao concluir a avaliacao completa por CBO habilitado (Quadro 07 da Nota C4).

## Legislacao e Normas de Referencia

* Brasil. Ministerio da Saude. Secretaria de Atencao Primaria a Saude. Nota Metodologica C4: cuidado da pessoa com diabetes. Brasilia, 2026.
* Brasil. Ministerio da Saude. Portaria SCTIE/MS no 13, de 21 de fevereiro de 2026. Protocolo Clinico e Diretrizes Terapeuticas do Diabete Melito Tipo 2.
* International Working Group on the Diabetic Foot (IWGDF). Guidelines on the prevention and management of diabetes-related foot disease, 2023.
* Sociedade Brasileira de Diabetes (SBD). Diretriz de Diagnostico e Prevencao de Ulceras no Pe Diabetico, 2026.
* Brasil. Lei no 13.709, de 14 de agosto de 2018. Lei Geral de Protecao de Dados Pessoais (LGPD).
* Wazlawick, R. S. et al. Desenvolvimento de Software Centrado no Usuario. Universidade Federal de Santa Catarina, 2025.
