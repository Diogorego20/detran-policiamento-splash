📄 PDF Split Pro - Divisor Inteligente de Arquivos PDF
https://img.shields.io/badge/Version-1.0.0-blue
https://img.shields.io/badge/R-4.0%252B-brightgreen
https://img.shields.io/badge/Shiny-Web%2520App-orange

🎯 Sobre o Projeto
PDF Split Pro é uma solução inteligente desenvolvida para resolver um problema comum no dia a dia de profissionais, estudantes e organizações: a necessidade de dividir arquivos PDF grandes em partes menores para atender limites de tamanho em sistemas corporativos, portais governamentais e plataformas de envio.

"Essa tarefa é muito desgastante já que não temos a capacidade de ser acertivo ao mensurar qual parte vai em que e se essa parte escolhida ultrapassou ou está dentro do parâmetro de 10MB" - Diogo Rego, Estudante de Estatística

✨ Funcionalidades Principais
🚀 Divisão Inteligente
Divisão Automática: Algoritmo inteligente que calcula automaticamente a melhor forma de dividir o PDF

Limite Personalizável: Partes de até 10MB (configurável)

Suporte a Grandes Arquivos: Processa arquivos de até 1GB sem problemas

📊 Interface Amigável
Aplicativo Web: Interface Shiny moderna e responsiva

Upload Simples: Arraste e solte ou selecione o arquivo

Feedback Visual: Barra de progresso e status em tempo real

📈 Análise Detalhada
Pré-análise: Mostra tamanho original e número de páginas antes da divisão

Relatório Detalhado: Tabela com informações de cada parte criada

Estatísticas Completas: Gráficos e métricas do processo

💾 Exportação Facilitada
Download em ZIP: Todas as partes compactadas em um único arquivo

Numeração Automática: Partes nomeadas sequencialmente (parte_01, parte_02, etc.)

Metadados Preservados: Mantém a qualidade e propriedades originais do PDF

🛠️ Tecnologias Utilizadas
Tecnologia	Função	Versão
R	Linguagem principal	4.0+
Shiny	Framework web	1.7+
pdftools	Manipulação de PDFs	3.3+
qpdf	Divisão eficiente	1.2+
fs	Gerenciamento de arquivos	1.5+
📥 Instalação e Uso
Pré-requisitos
R (versão 4.0 ou superior)

RStudio (recomendado)

Método 1: Aplicativo Web (Recomendado)
r
# 1. Instalar pacotes necessários
install.packages(c("shiny", "shinythemes", "pdftools", "fs", "qpdf", "DT", "zip"))

# 2. Executar o aplicativo
shiny::runGitHub("pdf-split-pro", "seu-usuario")
Método 2: Versão Local
r
# Copiar e colar o código completo no RStudio
# Executar todo o script
# O aplicativo abrirá automaticamente no navegador
Método 3: Linha de Comando
r
source("https://raw.githubusercontent.com/seu-usuario/pdf-split-pro/main/pdf_splitter.R")
🎮 Como Usar
Passo a Passo Simples:
Acesse o aplicativo em http://127.0.0.1:XXXX

Selecione seu arquivo PDF (até 1GB)

Defina o tamanho máximo por parte (padrão: 10MB)

Clique em "Processar PDF"

Aguarde o processamento (barra de progresso)

Faça download do ZIP com todas as partes

Exemplo de Saída:
text
📁 Arquivo Original: relatorio_final.pdf (85.3 MB)
🎯 Divisão em: 9 partes de ~9.5 MB cada
📊 Partes Criadas:
   • parte_01.pdf (9.2 MB) - páginas 1-45
   • parte_02.pdf (9.4 MB) - páginas 46-90
   • parte_09.pdf (8.7 MB) - páginas 396-440
🏗️ Estrutura do Projeto
text
pdf-split-pro/
├── app.R                 # Aplicativo Shiny principal
├── pdf_functions.R       # Funções de divisão de PDF
├── www/
│   ├── style.css         # Estilos customizados
│   └── script.js         # JavaScript adicional
├── examples/
│   └── exemplo_uso.R     # Exemplos de uso
├── README.md             # Este arquivo
└── LICENSE               # Licença do projeto
📊 Casos de Uso Típicos
🏢 Setor Público
Documentos do DETRAN: Laudos e relatórios de policiamento

Processos Administrativos: Envio para sistemas governamentais

Licitações: Documentação de editais e propostas

🎓 Ambiente Acadêmico
TCCs e Dissertações: Materiais complementares grandes

Artigos Científicos: Anexos e suplementos

Projetos de Pesquisa: Relatórios técnicos extensos

💼 Corporativo
Relatórios Anuais: Demonstrações financeiras

Manuais Técnicos: Documentação de produtos

Propostas Comerciais: Apresentações detalhadas

🔧 Solução de Problemas
Problemas Comuns:
Arquivo muito grande: Suporte até 1GB garantido

PDF protegido: Necessidade de senha de edição

Falha no processamento: Verificar integridade do arquivo

Logs e Debug:
r
# Ativar modo debug
options(shiny.trace = TRUE)

# Verificar logs do processamento
cat("🔍 Debug: Iniciando divisão do arquivo...")
🤝 Contribuição
Contribuições são bem-vindas! Areas de melhoria:

Suporte a PDFs criptografados

Interface em múltiplos idiomas

Integração com nuvem (Google Drive, Dropbox)

API REST para integração

Como contribuir:
Fork o projeto

Crie uma branch para sua feature (git checkout -b feature/AmazingFeature)

Commit suas mudanças (git commit -m 'Add some AmazingFeature')

Push para a branch (git push origin feature/AmazingFeature)

Abra um Pull Request

📝 Licença
Distribuído sob licença MIT. Veja LICENSE para mais informações.

👨‍💻 Autor
Diogo Rego - Estudante de Estatística

GitHub: @diogorego

LinkedIn: Diogo Rego

Email: diogo.rego@example.com

🙏 Agradecimentos
Equipe do DETRAN-PB pelo feedback valioso

Comunidade R-Brasil pelo suporte técnico

Professores do curso de Estatística pela orientação
