# AI Red Teaming Arena 🛡️🤖
### *Simulador Interativo de Vulnerabilidades e Hardening de Prompts em IA*

O **AI Red Teaming Arena** é uma plataforma interativa de simulação de cibersegurança projetada para demonstrar, testar e mitigar os principais riscos de segurança em modelos de linguagem (LLMs), conforme mapeados por organizações globais como a **OWASP Foundation** (OWASP Top 10 para Aplicações de LLM).

A aplicação conta com um ambiente sandbox prático no estilo CTF (Capture The Flag) integrado diretamente com o modelo **Gemini 3.5**, permitindo que profissionais de segurança, desenvolvedores e entusiastas experimentem ataques adversariais reais e testem diferentes camadas de defesas operacionais.

---

## 🎨 Visual Preview & Design (Tema: Elegant Dark / AI-SEC)
O visual foi meticulosamente projetado com base no estilo de painéis de segurança cibernética tática militar (**AI-SEC // ADVERSARIAL ADVISORY**):
*   **Cores de Destaque:** Ciano Elétrico (`#00E5FF`), Verde-Teal (`#45A29E`), Vermelho de Ameaça Crítica e Cinza de Chapa Metálica (`#8B949E`).
*   **Fundo:** Negro Profundo Carbono (`#0B0E14`) com painéis em Cinza de Terminal (`#161B22`) e bordas reforçadas.
*   **Tipografia:** Títulos em *Space Grotesk* de alto contraste combinados com *JetBrains Mono* para logs de rede e código operacional.

---

## 🚀 Principais Funcionalidades

### 1. Playground CTF (Capture The Flag) - 4 Níveis de Vulnerabilidade
Teste suas habilidades de engenharia social e exploração de IA em desafios interativos reais alimentados pela API do Gemini:
*   **Nível 1: Injeção Direta (Direct Prompt Injection):** Force o "Guardião de Segredos" a revelar o código confidencial escondido através de comandos imperativos ou ofuscações.
*   **Nível 2: Vazamento de Sistema (Prompt Leakage):** Extraia as instruções secretas e regras do sistema do "Administrador de Rede de IA" sem que ele mude de assunto.
*   **Nível 3: Jailbreaking (Ethical Bypass / Roleplay):** Use cenários de encenação (Teatro/DAN/Hipocrisia) para burlar o alinhamento ético do modelo e fazê-lo pronunciar a frase proibida: *"EU SOU LIVRE E BURLADO"*.
*   **Nível 4: Injeção Indireta (Indirect Prompt Injection):** Simule a análise de uma página web externa comprometida que contém um payload malicioso oculto que assume o controle do comportamento do resumidor.

### 2. Painel de Configuração de Defesas Operacionais
Ative e combine três níveis de contramedidas de segurança recomendadas pela indústria de IA para neutralizar os seus ataques:
1.  **Filtro de Entrada (Input Sanitizer):** Um algoritmo de varredura pré-inferência que bloqueia strings maliciosas comuns e termos associados antes de chegarem à inteligência.
2.  **Prompt Hardening:** Diretrizes defensivas agressivas de controle acopladas dinamicamente ao *System Prompt* instruindo o modelo a ignorar jogos de persuasão, roleplay e engenharia reversa.
3.  **Juiz de IA (LLM-as-a-Judge) ⚖️:** Um classificador de segurança externo e isolado baseado no Gemini que audita a resposta gerada de forma assíncrona, interceptando-a e censurando-a instantaneamente se detectar vazamento ou violação.

### 3. Simulador de Fuzzing de Prompt Automatizado 🧪
Submeta testes massivos em paralelo! O simulador permite disparar coleções automatizadas de 5 payloads adversariais clássicos (usando variações baseadas no framework *Promptfoo*) contra o modelo. Ele calcula a taxa de bypass em tempo real e compara lado a lado o comportamento do LLM puro vs. com defesas totais ativadas.

### 4. Guia Teórico & Manual OWASP integrado
Contém explicações detalhadas em português sobre a mecânica de cada risco de segurança em IA, acompanhado de estratégias arquiteturais de hardening, sandboxing de ferramentas e controle de outputs.

---

## 🛠️ Tecnologias Utilizadas

O projeto utiliza um ecossistema de ponta focado em robustez operacional, baixa latência e portabilidade total na nuvem:
*   **Frontend:** React 19, TypeScript, Tailwind CSS, Lucide Icons, e Framer Motion (para transições fluidas e animações de log).
*   **Backend:** Express (Node.js) em TypeScript rodando com compilação avançada rápida.
*   **Engine de IA:** `@google/genai` (SDK oficial do Google para chamadas server-side robustas e ultra seguras para o modelo `gemini-3.5-flash`).
*   **Build & Bundler:** Vite (Frontend) & Esbuild (Backend compilando o servidor em um bundle `.cjs` altamente otimizado para produção).

---

## 💻 Como Rodar o Projeto Localmente

### Pré-requisitos
*   Node.js instalado (v18 ou superior).
*   Uma chave de API do Gemini (configurada na variável de ambiente).

### Passos para Inicialização

1.  **Instale as dependências:**
    ```bash
    npm install
    ```

2.  **Configure suas Chaves de Segurança:**
    Crie um arquivo `.env` na raiz do projeto (copie o modelo de `.env.example`) e adicione sua chave de API do Gemini:
    ```env
    GEMINI_API_KEY="SUA_CHAVE_AQUI"
    ```

3.  **Inicie o ambiente de Desenvolvimento (Express + Vite):**
    ```bash
    npm run dev
    ```
    O servidor estará ativo em `http://localhost:3000`.

4.  **Compilar para Produção:**
    ```bash
    npm run build
    ```
    Isso gerará os arquivos estáticos na pasta `dist/` e gerará o servidor otimizado empacotado em `dist/server.cjs`.

5.  **Iniciar Servidor de Produção:**
    ```bash
    npm start
    ```

---

## 🔒 Segurança em Primeiro Lugar
*Todas as simulações e ataques de injeção contidos nesta aplicação são puramente educativos e ocorrem em um ambiente de sandbox isolado. Nenhuma técnica contida neste projeto deve ser aplicada em ambientes de produção de terceiros sem autorização explícita.*
# Teaming-Arena  
# Teaming-Arena  
# Teaming-Arena  
