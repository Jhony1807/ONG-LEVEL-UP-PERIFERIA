# ONG-LEVEL-UP-PERIFERIA
trabalho acadêmico que descobre talentos de CS2 e VALORANT.

🎮 Instituto Level Up Periferia
Protótipo acadêmico desenvolvido como Projeto Integrador de Front-end, representando uma ONG fictícia focada em aproximar crianças e adolescentes de periferias ao cenário dos e-sports (Counter-Strike 2 e Valorant) através de treinos, suporte educacional e acompanhamento familiar.

👥 Desenvolvedores

<p><a href="https://www.linkedin.com/in/jonata-alves-borsari/" target="_blank" rel="noopener">Jonata Alves Borsari</a></p>
<br>
<p><a href="https://www.linkedin.com/in/joão-frazão-zanon/" target="_blank" rel="noopener">Joao Frazon Zanon</a></p>

🛠️ Tecnologias Utilizadas
HTML5: Estruturação semântica das páginas (<header>, <main>, <section>, <details>, <summary>).

CSS3: Estilização responsiva com variáveis (:root), Flexbox, CSS Grid e design adaptativo para dispositivos móveis (@media queries).

JavaScript (ES6+): Dinâmica de interface e validações de formulários no lado do cliente.

📂 Estrutura do Projeto
index.html — Página inicial com destaque institucional, números de impacto[cite: 5] e aviso acadêmico.

sobre.html — História da ONG, missão, público-alvo, galeria comparativa de lan houses e botão interativo[cite: 1].

projetos.html — Cartões explicativos dos pilares (Centro de Treino, Jogador Estudante e Liga da Quebrada)[cite: 6].

cs2.html — Página temática dedicada ao Counter-Strike 2 (história, jogabilidade e principais organizações)[cite: 3].

valorant.html — Página temática dedicada ao Valorant (história, agentes, VCT e organizações)[cite: 7].

contato.html — Canal de inscrição e voluntariado com formulário validado via JavaScript[cite: 2].

estilos.css — Folha de estilos centralizada e customizada por temas de jogos[cite: 4].

script.js — Script de controle de exibição de elementos institucionais[cite: 9].

formulario.js — Script de validação e tratamento de envio do formulário de contato[cite: 8].

⚙️ Verificações e Funcionalidades do JavaScript
O projeto conta com duas principais funcionalidades em JavaScript puro (Vanilla JS), estruturadas para garantir acessibilidade, interatividade e validação robusta de dados:

1. Validação de Formulário e Feedback Visual (formulario.js)
Atua na página de contato (contato.html) interceptando o evento de envio (submit) para validar as entradas do usuário antes de simular o processamento[cite: 8].

Prevenção de Recarregamento: Utiliza evento.preventDefault() para barrar o comportamento padrão de submissão do formulário[cite: 8].

Limpeza de Dados: Aplica o método .trim() para remover espaços em branco desnecessários nas pontas dos textos digitados[cite: 8].

Regras de Validação Verificadas passo a passo (if / else if):

Campos Obrigatórios: Verifica se há campos vazios (nome, email, assunto, mensagem)[cite: 8].

Tamanho Mínimo do Nome: Exige que o nome possua pelo menos 3 caracteres[cite: 8].

Validação Nativa de E-mail: Utiliza a verificação integrada do HTML5 (campoEmail.checkValidity()) combinada ao script para garantir formatos válidos (ex: nome@email.com)[cite: 8].

Seleção de Jogo: Assegura que o usuário selecionou uma opção válida no elemento <select>[cite: '8'].

Tamanho da Mensagem: Exige que o campo de texto da mensagem contenha no mínimo 10 caracteres[cite: 8].

Feedback Dinâmico: Caso encontre erros, exibe mensagens explicativas com classes de alerta (.erro). Se todas as validações forem bem-sucedidas, exibe uma mensagem de confirmação (.ok), insere dinamicamente o nome do jogo escolhido e limpa os campos através de formulario.reset()[cite: 8].

2. Painel Dinâmico de Informações Institucionais (script.js)
Atua na página "Sobre" (sobre.html), permitindo alternar a visibilidade de conteúdos adicionais sob demanda[cite: 9].

Alternância de Estados (Toggle): Verifica através de uma estrutura condicional (if / else) se o painel extra está oculto (display: "none") ou visível (display: "block")[cite: 9].

Modificação de Texto e Acessibilidade:

Altera dinamicamente o textContent do botão entre "Ver informações institucionais" e "Ocultar informações"[cite: 9].

Atualiza os atributos ARIA (aria-expanded="true/false") para assegurar acessibilidade correta a leitores de tela[cite: 9].

🚀 Como Executar o Projeto Localmente
Clone este repositório para a sua máquina:

Bash
git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
(Substitua SEU-USUARIO/NOME-DO-REPOSITORIO pelo link real do seu repositório no GitHub).

Abra a pasta do projeto no seu editor de código preferido (como o VS Code).

Instale a extensão Live Server no VS Code (opcional, mas recomendado).

Clique com o botão direito em index.html e selecione "Open with Live Server" (ou abra o arquivo diretamente no seu navegador web).
