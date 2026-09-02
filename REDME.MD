# 1. O "Contexto Base" para colar no início de um novo chat
Para que o modelo já responda exatamente dentro do padrão visual do seu projeto (sem ter que reexplicar classes ou design), você pode iniciar a conversa enviando uma introdução direta como esta:

"Tenho um portal de procedimentos no GitHub Pages com tema claro estilo Google/Gemini. Uso as classes .container, .doc-header, .stepper, .step, .step-last, .step-subtitle, .step-img e blocos de código <code></code>. O arquivo CSS fica em ../css/style.css. Quero criar um novo procedimento..."

# 2. As informações necessárias para criar um novo procedimento
Sempre que você quiser documentar uma rotina nova, você só precisa fornecer:

Título e Categoria: (Ex.: Hyper-V, PowerShell, Redes, etc.).

Rascunho bruto dos passos: Pode ser apenas anotações soltas, a lista do que você fez no terminal ou uma sequência de tópicos.

Comandos utilizados: Códigos de PowerShell, CMD, Bash, etc.

Pontos de atenção / Alertas: O que não pode ser feito ou o que precisa de cuidado para não quebrar o ambiente.

Onde haverá imagens: Basta avisar onde você pretende colocar prints (ex: "aqui vai uma imagem chamada pasta_vm.png").

# Sugestões de melhorias futuras para o portal
Quando quiser evoluir a página de procedimentos, algumas ideias que agregam valor:

Botão "Copiar" nos blocos de código: Adicionar um pequeno script em JavaScript que coloca um botão discreto de "Copiar" no canto de cada caixa de código, facilitando a execução de comandos sem precisar selecionar texto no celular.

Barra de Pesquisa no index.html: Um filtro em tempo real na página inicial para encontrar procedimentos digitando palavras-chave (ex: "VHDX", "Backup", "NAT").

Snippet no VS Code: Criar um atalho no editor para que, ao digitar doc-pop e apertar Tab, a estrutura inteira do HTML (com header, stepper e container) seja criada automaticamente em segundos.

Estilo para Impressão / PDF (@media print): Ajustar o CSS para que, ao pressionar Ctrl + P no navegador, ele gere um relatório em PDF limpo, sem botões de navegação, pronto para envio ou arquivamento formal.