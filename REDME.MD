# Prompt para o Gemini


```text
Atue como desenvolvedor front-end. Preciso gerar uma nova página HTML para o meu portal de procedimentos técnicos (GitHub Pages).

REGRAS OBRIGATÓRIAS DE ESTRUTURA:
1. CSS: Linkar sempre com <link rel="stylesheet" href="../css/style.css">
2. Estrutura e Cabeçalho:
   - Imediatamente após <body>, incluir o rodapé de impressão:
     <div class="print-footer-all"><span><strong>Elaborado por:</strong> Gustavo Vieira Ermelino &bull; e-mail: g3gustavo@gmail.com</span></div>
   - <div class="container"> envolvendo todo o conteúdo
   - Barra de ações logo no início do container:
     <div class="doc-actions">
         <a href="../index.html" class="nav-back">← Voltar aos procedimentos</a>
         <button onclick="window.print()" class="btn-print">🖨️ Salvar em PDF / Imprimir</button>
     </div>
   - <header class="doc-header"> com <h1> e <p class="subtitle">
3. Stepper e Passos:
   - <main class="stepper"> contendo os passos
   - Cada passo normal usa <div class="step"> com <h3> e <p class="step-subtitle">
   - O ÚLTIMO passo DEVE usar <div class="step step-last">
4. Componentes visuais:
   - Comandos/terminal: usar <pre><code>...</code></pre>
   - Variáveis/termos técnicos: usar <code>...</code> em linha
   - Tabelas: SEMPRE envolver em <div class="table-responsive"><table>...</table></div>
   - Alertas críticos: <div class="alert-box danger">...</div>
   - Avisos/atenção: <div class="callout warning">...</div>
   - Notas informativas: <p class="info-note">...</p>
   - Imagens: usar <img class="step-img" src="..." alt="...">
5. Saída: Apenas o código HTML completo, pronto para salvar no arquivo.

DADOS DO NOVO PROCEDIMENTO:
- Título: [Digite aqui o título]
- Subtítulo: [Resumo de 1 linha]
- Conteúdo bruto / passos:
[Cole aqui o conteúdo, comandos ou texto do Word]
```

# Sugestões de melhorias futuras para o portal
Quando quiser evoluir a página de procedimentos, algumas ideias que agregam valor:

- [ ] Botão "Copiar" nos blocos de código: Adicionar um pequeno script em JavaScript que coloca um botão discreto de "Copiar" no canto de cada caixa de código, facilitando a execução de comandos sem precisar selecionar texto no celular.

- [ ] Barra de Pesquisa no index.html: Um filtro em tempo real na página inicial para encontrar procedimentos digitando palavras-chave (ex: "VHDX", "Backup", "NAT").

- [ ] Snippet no VS Code: Criar um atalho no editor para que, ao digitar doc-pop e apertar Tab, a estrutura inteira do HTML (com header, stepper e container) seja criada automaticamente em segundos.

- [x] Estilo para Impressão / PDF (@media print): Implementado com botão de impressão nativo, ocultação de menus na folha, preservação de cores via CSS e rodapé padronizado em todas as páginas.