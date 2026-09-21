# 🎯 JobMatch ATS — Otimizador Semântico de Currículos

> Aplicação web desenvolvida no **Lovable** que diagnostica a compatibilidade entre currículos e descrições de vagas frente aos filtros de sistemas ATS (Applicant Tracking Systems), gerando versões reestruturadas sem fabricar dados.

🔗 **Aplicação no ar:** (https://jobmatch-joaot.lovable.app)

---

## 📌 1. Qual problema a aplicação resolve?

Milhares de candidatos qualificados são descartados sumariamente na primeira triagem dos processos seletivos. O motivo não costuma ser a falta de competência, mas sim a incompatibilidade técnica com os softwares de **ATS (Applicant Tracking Systems)** — robôs que ranqueiam perfis antes que um recrutador humano veja o documento.

Diferenças de nomenclatura (ex.: usar *"construção de APIs"* em vez de *"RESTful Web APIs"* exigido na vaga), layouts inadequados e ausência de termos essenciais derrubam a pontuação do candidato.

O **JobMatch ATS** equaliza essa disputa ao:
- Fazer o cruzamento semântico entre o anúncio da vaga e o perfil do candidato.
- Expor claramente quais termos mandatórios estão presentes e quais estão em falta.
- Reformatar o currículo em padrões limpos de leitura de máquina.
- **Respeitar a ética profissional:** a ferramenta calibra o vocabulário e o destaque das atribuições reais, sem inventar experiências que o candidato não possui.

---

## 🤖 2. O Mega Prompt Utilizado

Para a geração do MVP, foi utilizado o seguinte prompt estruturado em Markdown no Lovable:

```txt
Crie uma aplicação web moderna chamada "JobMatch ATS" para otimizar currículos contra sistemas de rastreamento de candidatos (ATS). A aplicação deve ser responsiva, com visual SaaS minimalista e profissional utilizando componentes do Shadcn UI e Tailwind CSS (paleta em tons de Slate escuro/cinza neutro, com Indigo como cor primária e detalhes em Esmeralda e Rose).

### Princípio Ético Inegociável (Destaque visual na interface)
Exiba um banner ou aviso no topo: 
"Transparência e Ética: Esta ferramenta ajusta a semântica, formatação e relevância de palavras-chave do seu currículo. Ela NUNCA inventa competências, cargos ou experiências que você não possui."

### Funcionalidades e Telas:
1. Cabeçalho (Header):
- Logotipo com ícone de documento/matching ("JobMatch ATS").
- Botão "Carregar Exemplo" (preenche automaticamente a vaga e o currículo com dados de teste).
2. Área de Entrada de Dados:
- Textarea para descrição da vaga e Textarea para o currículo atual.
- Botão de análise com estado animado de processamento.
3. Painel de Resultados:
- Score de compatibilidade (0 a 100%).
- Tags de termos encontrados (verde) e ausentes (vermelho/âmbar).
- Checklist de boas práticas de legibilidade ATS.
4. Visualizador do Currículo Otimizado:
- Versão reescrita, organizada por seções padronizadas.
- Botões de "Copiar Texto" e "Exportar / Imprimir em PDF".
