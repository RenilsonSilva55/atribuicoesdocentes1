<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Atribuições dos Professores - Afya Medicina</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" xintegrity="sha512-Fo3rlrZj/k7ujTnHg4CGR2D7kSs0V4LLanw2qksYuRlEzO+tcaEPQogQ0KaoGN26/zrn20ImR1DfuLWnOo7aBA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            color: #333;
        }
        .card {
            background-color: #fff;
            border-radius: 1rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.2s ease-in-out;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .section-title {
            border-bottom: 2px solid #E91E63;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
            color: #E91E63;
            animation: fadeIn 1s ease-in-out;
        }
        .task-icon {
            color: #E91E63;
            margin-right: 1rem;
            font-size: 1.5rem;
            flex-shrink: 0;
            animation: pulse 2s infinite;
        }
        .game-container {
            padding: 1.5rem;
            background-color: #f0f2f5;
            border-radius: 1rem;
            box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.06);
            margin-top: 1rem;
            text-align: center;
            cursor: pointer;
            min-height: 150px;
            transition: background-color 0.3s;
        }
        .game-container:hover {
            background-color: #e2e8f0;
        }
        .task-list-item {
            animation: popIn 0.5s ease-out;
            transform-origin: center;
        }
        .rotate-in {
            animation: rotateIn 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        .flip-card {
            background-color: transparent;
            width: 100%;
            height: 150px;
            perspective: 1000px;
        }
        .flip-card-inner {
            position: relative;
            width: 100%;
            height: 100%;
            text-align: center;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        .flip-card.flipped .flip-card-inner {
            transform: rotateY(180deg);
        }
        .flip-card-front, .flip-card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
            border-radius: 1rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .flip-card-front {
            background-color: #f0f2f5;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            color: #4b5563;
        }
        .flip-card-back {
            background-color: #f0f2f5;
            color: #333;
            transform: rotateY(180deg);
            padding: 1rem;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            justify-content: center;
        }
        .task-item-flip {
            animation: popIn 0.5s ease-out;
        }
        .quiz-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: left;
            padding: 1.5rem;
            background-color: #e2e8f0;
            border-radius: 1rem;
            margin-top: 1rem;
            width: 100%;
        }
        .quiz-question {
            font-weight: 600;
            margin-bottom: 1rem;
            color: #E91E63;
        }
        .quiz-option {
            background-color: #fff;
            padding: 0.5rem 1rem;
            border-radius: 0.5rem;
            margin-bottom: 0.5rem;
            cursor: pointer;
            transition: background-color 0.2s, transform 0.1s;
            width: 100%;
        }
        .quiz-option:hover {
            background-color: #f0f2f5;
            transform: scale(1.02);
        }
        .correct {
            background-color: #d1fae5;
        }
        .incorrect {
            background-color: #fecaca;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes popIn {
            from { opacity: 0; transform: scale(0.5); }
            to { opacity: 1; transform: scale(1); }
        }
        @keyframes rotateIn {
            from { opacity: 0; transform: rotateY(90deg) scale(0.8); }
            to { opacity: 1; transform: rotateY(0deg) scale(1); }
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body class="p-4 sm:p-8">
    <div class="max-w-6xl mx-auto bg-white p-6 sm:p-10 rounded-2xl shadow-lg">
        <header class="text-center mb-10">
            <img src="https://placehold.co/250x50/E91E63/ffffff?text=Afya+Faculdade+Redenção.+PA." alt="Logo Afya Faculdade Redenção. PA." class="mx-auto mb-4 rounded-lg">
            <h1 class="text-3xl sm:text-4xl font-extrabold text-gray-800 mb-2">Atribuições dos Professores</h1>
            <p class="text-lg text-gray-600">Material de instrução para Professores Focais Administrativos, Especialistas Locais dos Eixos e Docentes dos Módulos da Matriz Curricular de Medicina</p>
        </header>
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Professor Focal Administrativo</h2>
            <p class="text-gray-700 mb-6">O professor focal administrativo é responsável pela organização e gestão dos registros acadêmicos do módulo sob sua responsabilidade, garantindo a fluidez e precisão das informações.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Dinâmica 1: Organização do Ambiente Virtual (CANVAS) -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-desktop task-icon"></i> Organização do Ambiente Virtual (CANVAS)</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar as tarefas!</p>
                    <div id="game-canvas-tasks" class="game-container flex-col cursor-pointer">
                        <p id="game-canvas-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
                <!-- Dinâmica 2: Lançamento de Avaliações e Frequência (RM) -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-clipboard-check task-icon"></i> Lançamento e Gestão de Avaliações e Frequência (RM)</h3>
                    <p class="text-gray-600 mb-4">Clique no ícone para lançar as notas!</p>
                    <div class="game-container flex-col">
                        <div id="game-rm-tasks-display" class="flex flex-col items-center justify-center">
                            <button id="game-rm-button" class="text-6xl text-[#E91E63] animate-pulse transition-transform duration-300 transform hover:scale-110">
                                <i class="fas fa-sync-alt rotate-in"></i>
                            </button>
                            <p id="game-rm-prompt" class="text-gray-500 text-lg font-semibold mt-4">Clique para lançar!</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Seção: Especialista Local do Eixo -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Especialista Local do Eixo</h2>
            <p class="text-gray-700 mb-6">O Especialista Local do Eixo atua como modelo para os demais docentes, sendo responsável por planejar e acompanhar a matriz curricular do curso.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Dinâmica 3: Planejamento e Acompanhamento Pedagógico -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-tasks task-icon"></i> Planejamento e Acompanhamento Pedagógico</h3>
                    <p class="text-gray-600 mb-4">Clique no cartão para virar e ver os tópicos!</p>
                    <div class="flip-card cursor-pointer" onclick="this.classList.toggle('flipped')">
                        <div class="flip-card-inner">
                            <div class="flip-card-front">
                                <p>Clique para revelar!</p>
                            </div>
                            <div class="flip-card-back">
                                <ul class="text-left space-y-2 w-full">
                                    <li class="task-list-item text-gray-800 text-sm p-2 bg-white rounded-lg shadow-md w-full"><i class="fas fa-check-circle text-[#E91E63] mr-2"></i>Acompanhar a execução da matriz nas IES.</li>
                                    <li class="task-list-item text-gray-800 text-sm p-2 bg-white rounded-lg shadow-md w-full"><i class="fas fa-check-circle text-[#E91E63] mr-2"></i>Revisar manuais dos professores e dar feedback.</li>
                                    <li class="task-list-item text-gray-800 text-sm p-2 bg-white rounded-lg shadow-md w-full"><i class="fas fa-check-circle text-[#E91E63] mr-2"></i>Fazer a gestão dos GAPs de aprendizagem.</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Dinâmica 4: Articulação e Desenvolvimento -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-sitemap task-icon"></i> Articulação e Desenvolvimento</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-articulacao-tasks" class="game-container flex-col">
                        <p id="game-articulacao-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
                <!-- Dinâmica 5: Reuniões e Colaboração -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-handshake task-icon"></i> Reuniões e Colaboração</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-reunioes-tasks" class="game-container flex-col">
                        <p id="game-reunioes-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
            </div>
        </section> <!-- Dinâmica Extra: Tabela de Atribuições e CH -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">ESPECIALISTAS LOCAIS DOS EIXOS | CH + ATRIBUIÇÕES</h2>
            <p class="text-gray-700 mb-6">Visão geral da carga horária e atribuições dos Especialistas Locais de Eixo por módulo. Clique para revelar os detalhes!</p>
            <div id="tabela-atribuicoes-dinamica" class="card p-6 cursor-pointer">
                <div id="tabela-prompt" class="text-center text-gray-500 text-lg font-semibold">
                    <p>Clique para ver a tabela!</p>
                    <p class="text-sm mt-2">(As informações serão apresentadas em um formato de tabela dinâmica.)</p>
                </div>
                <div id="tabela-conteudo" class="overflow-x-auto hidden">
                    <table class="min-w-full bg-white rounded-lg shadow-md mt-4">
                        <thead class="bg-[#E91E63] text-white">
                            <tr>
                                <th class="py-2 px-4">Módulo</th>
                                <th class="py-2 px-4">Carga Horária</th>
                                <th class="py-2 px-4">Atribuições</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td class="border px-4 py-2 text-center">SOI</td>
                                <td class="border px-4 py-2 text-center">20h (P1 a P2) | 10h (P3 a P5)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                            <tr class="bg-gray-50">
                                <td class="border px-4 py-2 text-center">MCM</td>
                                <td class="border px-4 py-2 text-center">8h (P1 a P5)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                            <tr>
                                <td class="border px-4 py-2 text-center">HAM</td>
                                <td class="border px-4 py-2 text-center">20h (P1 a P5) | 12h (P6 a P8)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                             <tr class="bg-gray-50">
                                <td class="border px-4 py-2 text-center">IESC</td>
                                <td class="border px-4 py-2 text-center">12h (P1 a P5) | 8h (P6 a P8)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                            <tr>
                                <td class="border px-4 py-2 text-center">PIEPE</td>
                                <td class="border px-4 py-2 text-center">8h (P1 a P5) | 4h (P6 a P8)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                             <tr class="bg-gray-50">
                                <td class="border px-4 py-2 text-center">CI</td>
                                <td class="border px-4 py-2 text-center">12h (P6 a P8)</td>
                                <td class="border px-4 py-2">Acompanhar a execução da matriz nas IES, revisar manuais, dar feedback e gerir GAPs de aprendizagem.</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </section>
        <!-- Dinâmica extra: Fluxo de Alinhamentos -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Fluxo de alinhamentos e ajustes</h2>
            <p class="text-gray-700 mb-6">Entenda o fluxo de colaboração entre os especialistas locais e a equipe pedagógica. Clique para revelar o fluxo!</p>
            <div id="fluxo-dinamica" class="card p-6 cursor-pointer">
                <div id="fluxo-prompt" class="text-center text-gray-500 text-lg font-semibold">
                    <p>Clique para ver o fluxo de alinhamentos!</p>
                </div>
                <div id="fluxo-conteudo" class="overflow-x-auto hidden">
                    <table class="min-w-full bg-white rounded-lg shadow-md mt-4">
                        <thead class="bg-[#E91E63] text-white">
                            <tr>
                                <th class="py-2 px-4 text-center">DA DIRETORIA</th>
                                <th class="py-2 px-4 text-center">PARA IES</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td class="border px-4 py-2 text-center align-top">
                                    <div class="flex flex-col items-center justify-center space-y-2">
                                        <div class="flex items-center space-x-2">
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">DIRETORIA DE MEDICINA</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">Gerente NAPED</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">Especialista em Ensino</div>
                                        </div>
                                        <i class="fas fa-arrow-down text-[#E91E63]"></i>
                                        <div class="bg-gray-200 p-2 rounded-lg text-sm text-center">NAPED Local</div>
                                    </div>
                                </td>
                                <td class="border px-4 py-2 text-center align-top">
                                    <div class="flex flex-col items-center justify-center space-y-2">
                                        <div class="flex items-center space-x-2">
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">ESPECIALISTAS NACIONAIS DOS EIXOS</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">SOI</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">HAM</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">IESC</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">PIEPE</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">CI</div>
                                            <div class="bg-[#E91E63] text-white p-2 rounded-lg text-sm">MCM/TCC</div>
                                        </div>
                                        <i class="fas fa-arrow-down text-[#E91E63]"></i>
                                        <div class="bg-gray-200 p-2 rounded-lg text-sm text-center">Especialistas Locais dos Eixos</div>
                                    </div>
                                </td>
                            </tr>
                            <tr>
                                <td colspan="2" class="border px-4 py-2 text-center align-top bg-gray-50">
                                     <div class="flex flex-col items-center justify-center space-y-2">
                                        <p class="text-sm font-semibold">Fluxo de colaboração:</p>
                                        <div class="flex flex-col md:flex-row items-center justify-center space-y-4 md:space-y-0 md:space-x-8">
                                            <div class="bg-gray-100 p-4 rounded-lg shadow-md text-sm text-center border">
                                                <p>A partir de encontros regulares, NAPED e ESPECIALISTAS DOS EIXOS dialogarão sobre os aspectos didáticos e pedagógicos a serem desenvolvidos pelo corpo docente da IES.</p>
                                            </div>
                                            <i class="fas fa-arrow-right text-[#E91E63]"></i>
                                            <div class="bg-gray-100 p-4 rounded-lg shadow-md text-sm text-center border">
                                                <p>Especialistas passam a ter funções de mapear e entender o status de maturação dos docentes.</p>
                                            </div>
                                            <i class="fas fa-arrow-right text-[#E91E63]"></i>
                                            <div class="bg-gray-100 p-4 rounded-lg shadow-md text-sm text-center border">
                                                <p>NAPED terá função de preparar e organizar a qualificação por eixos.</p>
                                            </div>
                                            <i class="fas fa-arrow-right text-[#E91E63]"></i>
                                            <div class="bg-gray-100 p-4 rounded-lg shadow-md text-sm text-center border">
                                                <p>Juntos, ofertarão momentos de desenvolvimento (capacitações/oficinas).</p>
                                            </div>
                                        </div>
                                    </div>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </section>
        <!-- Seção: Dinâmicas para Docentes dos Módulos -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Docentes dos Módulos</h2>
            <p class="text-gray-700 mb-6">Os docentes são peças-chave na manutenção dos registros acadêmicos e na garantia da qualidade do ensino.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Dinâmica 6: Avaliação Diária e por Competência -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-star task-icon"></i> Avaliação Diária e por Competência</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-avaliacao-tasks" class="game-container flex-col">
                        <p id="game-avaliacao-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
                <!-- Dinâmica 7: Frequência e Participação -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-user-check task-icon"></i> Frequência e Participação</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-frequencia-tasks" class="game-container flex-col">
                        <p id="game-frequencia-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
                <!-- Dinâmica 8: Lançamento de notas e frequências no sistema acadêmico -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-edit task-icon"></i> Lançamento de Notas e Frequências</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-lancamento-tasks" class="game-container flex-col">
                        <p id="game-lancamento-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
            </div>
        </section>
        <!-- Seção: Deveres e Obrigações Comuns -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Deveres e Obrigações Comuns a Todos os Docentes</h2>
            <p class="text-gray-700 mb-6">Além das atribuições específicas, todos os docentes do curso de Medicina devem cumprir as normas estabelecidas.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Dinâmica 9: Planejamento e Execução Didático-Pedagógica -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-chalkboard-teacher task-icon"></i> Planejamento e Execução Didático-Pedagógica</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-pedagogica-tasks" class="game-container flex-col">
                        <p id="game-pedagogica-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
                <!-- Dinâmica 10: Compromisso com a Qualidade Acadêmica -->
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-award task-icon"></i> Compromisso com a Qualidade Acadêmica</h3>
                    <p class="text-gray-600 mb-4">Clique no espaço abaixo para revelar os tópicos!</p>
                    <div id="game-qualidade-tasks" class="game-container flex-col">
                        <p id="game-qualidade-prompt" class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
            </div>
        </section>
        <!-- Seção de Quizzes Interativos -->
        <section class="mb-12">
            <h2 class="text-2xl sm:text-3xl font-bold section-title mb-6">Quizzes Interativos: Teste seu Conhecimento!</h2>
            <p class="text-gray-700 mb-6">Responda às perguntas para reforçar os principais pontos das atribuições docentes.</p>          
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Quiz 1: Professor Focal Administrativo -->
                <div class="card p-6 flex flex-col items-center justify-center">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-desktop text-[#E91E63] mr-2"></i> Quiz do Professor Focal</h3>
                    <div id="quiz-focal" class="quiz-container">
                        <!-- Pergunta e opções serão inseridas aqui via JS -->
                        <p class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>    
                <!-- Quiz 2: Especialista Local do Eixo -->
                <div class="card p-6 flex flex-col items-center justify-center">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-sitemap text-[#E91E63] mr-2"></i> Quiz do Especialista Local</h3>
                    <div id="quiz-especialista" class="quiz-container">
                        <p class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>          
                <!-- Quiz 3: Docentes dos Módulos -->
                <div class="card p-6 flex flex-col items-center justify-center">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4 flex items-center"><i class="fas fa-chalkboard-teacher text-[#E91E63] mr-2"></i> Quiz dos Docentes</h3>
                    <div id="quiz-docentes" class="quiz-container">
                        <p class="text-gray-500 text-lg font-semibold">Clique para começar!</p>
                    </div>
                </div>
            </div>
        </section>
        <footer class="text-center text-gray-500 mt-10 text-sm">
            <p>&copy; 2024 Afya. Todos os direitos reservados.</p>
        </footer>
    </div>
    <script> // Dados das tarefas por ID
        const tasks = {
            'game-canvas-tasks': [
                "Inserir o Plano de Ensino completo do módulo no CANVAS.",
                "Lançar as tarefas específicas do eixo (ex: SOI no pós-teste)."
            ],
            'game-rm-tasks': [
                "Compilar e lançar as notas finais de cada módulo no sistema acadêmico (RM).",
                "Lançar Conteúdo Previsto e Realizado.",
                "Registrar conteúdo ministrado e frequência em palestras.",
                "Registrar frequência nas avaliações e semanas de memorial."
            ],
            'game-articulacao-tasks': [
                "Promover o programa de desenvolvimento docente nas IES.",
                "Articular as ações locais com o NDE do curso."
            ],
            'game-reunioes-tasks': [
                "Participar de reuniões quinzenais com o Especialista Nacional.",
                "Participar de reuniões mensais com a Diretoria de Medicina."
            ],
            'game-avaliacao-tasks': [
                "Lançar diariamente as avaliações no CANVAS, utilizando a rubrica.",
                "Compilar avaliações e encaminhar ao professor focal."
            ],
            'game-frequencia-tasks': [
                "Acompanhar e registrar a frequência dos estudantes.",
                "Registrar o desempenho dos estudantes, quando aplicável."
            ],
            'game-lancamento-tasks': [
                "Registrar notas e frequência dos alunos conforme prazos."
            ],
            'game-pedagogica-tasks': [
                "Elaborar, cumprir e revisar planos de ensino alinhados ao PPC.",
                "Promover atividades que estimulem o pensamento crítico.",
                "Utilizar metodologias ativas e recursos atualizados."
            ],
            'game-qualidade-tasks': [
                "Zelar pela qualidade do ensino.",
                "Manter-se atualizado em sua área de conhecimento."
            ]
        };
        const quizzes = {
            'quiz-focal': {
                question: "Qual das tarefas abaixo é de responsabilidade do Professor Focal Administrativo?",
                options: [
                    "Revisar o plano de ensino do módulo.",
                    "Lançar as notas finais de cada módulo no sistema RM.",
                    "Elaborar itens de prova sob encomenda."
                ],
                correctAnswer: "Lançar as notas finais de cada módulo no sistema RM."
            },
            'quiz-especialista': {
                question: "A principal função do Especialista Local do Eixo é:",
                options: [
                    "Acompanhar o calendário acadêmico.",
                    "Atuar na gestão de registros acadêmicos no RM.",
                    "Planejar e acompanhar pedagogicamente a matriz curricular do curso."
                ],
                correctAnswer: "Planejar e acompanhar pedagogicamente a matriz curricular do curso."
            },
            'quiz-docentes': {
                question: "Qual é uma das obrigações comuns a todos os docentes do curso de Medicina?",
                options: [
                    "Manter postura ética e respeitosa com estudantes e colegas.",
                    "Ser o único responsável por todas as notas do módulo.",
                    "Aprovar a matriz curricular em reuniões."
                ],
                correctAnswer: "Manter postura ética e respeitosa com estudantes e colegas."
            }
        };
        const gameStates = {};
        const quizStates = {};
        function initGames() {
            for (const id in tasks) {
                gameStates[id] = false;
                const container = document.getElementById(id);
                if (container) {
                    container.addEventListener('click', () => showAllTasks(id));
                }
            }
            const rmButton = document.getElementById('game-rm-button');
            if (rmButton) {
                rmButton.addEventListener('click', () => showAllRmTasks());
            }
            for (const id in quizzes) {
                quizStates[id] = false;
                const container = document.getElementById(id);
                if (container) {
                    container.addEventListener('click', () => {
                        if (!quizStates[id]) {
                            showQuiz(id, container);
                        }
                    });
                }
            }
            // Dinâmica extra: Tabela de Atribuições
            const tabelaContainer = document.getElementById('tabela-atribuicoes-dinamica');
            if (tabelaContainer) {
                tabelaContainer.addEventListener('click', () => {
                    const tabelaConteudo = document.getElementById('tabela-conteudo');
                    const tabelaPrompt = document.getElementById('tabela-prompt');
                    tabelaPrompt.classList.add('hidden');
                    tabelaConteudo.classList.remove('hidden');
                    tabelaContainer.classList.remove('cursor-pointer');
                });
            }
            // Dinâmica extra: Fluxo de alinhamentos
            const fluxoContainer = document.getElementById('fluxo-dinamica');
            if (fluxoContainer) {
                fluxoContainer.addEventListener('click', () => {
                    const fluxoConteudo = document.getElementById('fluxo-conteudo');
                    const fluxoPrompt = document.getElementById('fluxo-prompt');
                    fluxoPrompt.classList.add('hidden');
                    fluxoConteudo.classList.remove('hidden');
                    fluxoContainer.classList.remove('cursor-pointer');
                });
            }
        }
        function showAllTasks(id) {
            if (gameStates[id]) return;
            const container = document.getElementById(id);
            const prompt = document.getElementById(`${id}-prompt`);     
            if (prompt) {
                prompt.classList.add('hidden');
            }   
            tasks[id].forEach(taskText => {
                const taskElement = document.createElement('div');
                taskElement.classList.add('task-list-item', 'text-gray-800', 'text-sm', 'my-2', 'p-2', 'bg-white', 'rounded-lg', 'shadow-md', 'w-full');
                taskElement.innerHTML = `<i class="fas fa-check-circle text-green-500 mr-2"></i>${taskText}`;
                container.appendChild(taskElement);
            });
            gameStates[id] = true;
        }
        function showAllRmTasks() {
            const id = 'game-rm-tasks';
            if (gameStates[id]) return;
            const displayArea = document.getElementById('game-rm-tasks-display');
            const rmButton = document.getElementById('game-rm-button');
            const rmPrompt = document.getElementById('game-rm-prompt');
            if (rmButton) rmButton.disabled = true;
            if (rmPrompt) rmPrompt.classList.add('hidden');
            tasks[id].forEach(taskText => {
                const taskElement = document.createElement('div');
                taskElement.classList.add('task-list-item', 'text-gray-800', 'text-sm', 'my-2', 'p-2', 'bg-white', 'rounded-lg', 'shadow-md', 'w-full', 'rotate-in');
                taskElement.innerHTML = `<i class="fas fa-check-circle text-green-500 mr-2"></i>${taskText}`;
                displayArea.appendChild(taskElement);
            });
            gameStates[id] = true;
        }
        function showQuiz(id, container) {
            if (quizStates[id]) return;
            quizStates[id] = true;
            container.innerHTML = '';
            container.classList.remove('cursor-pointer');
            container.classList.add('bg-white');
       const quizData = quizzes[id];   
            const questionElement = document.createElement('p');
            questionElement.classList.add('quiz-question');
            questionElement.textContent = quizData.question;
            container.appendChild(questionElement);
            const optionsContainer = document.createElement('div');
            optionsContainer.classList.add('w-full');
            shuffle(quizData.options).forEach(optionText => {
                const optionElement = document.createElement('button');
                optionElement.classList.add('quiz-option');
                optionElement.textContent = optionText;
                optionElement.addEventListener('click', () => checkQuizAnswer(optionElement, optionText, quizData.correctAnswer, optionsContainer));
                optionsContainer.appendChild(optionElement);
            });
            container.appendChild(optionsContainer);
        }
        function checkQuizAnswer(selectedElement, selectedAnswer, correctAnswer, optionsContainer) {
            const options = optionsContainer.querySelectorAll('.quiz-option');
            options.forEach(option => option.disabled = true);
            if (selectedAnswer === correctAnswer) {
                selectedElement.classList.add('correct');
            } else {
                selectedElement.classList.add('incorrect');
                options.forEach(option => {
                    if (option.textContent === correctAnswer) {
                        option.classList.add('correct');
                    }
                });
            }
        }
        function shuffle(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
            return array;
        }
        window.onload = initGames;
    </script>
</body>
</html>
