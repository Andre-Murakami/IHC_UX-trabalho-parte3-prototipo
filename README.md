Market Pulse - Guia de Teste do protótipo
Guia rápido de uso

----------------------------------------------------------------
ATENÇÃO: Antes de tudo 
----------------------------------------------------------------
⚠️ IMPORTANTE: Este é um protótipo acadêmico. Não usar senhas reais. 
   Dados armazenados localmente no navegador.


----------------------------------------------------------------
PASSO 0: 🔧 Requisitos Técnicos
----------------------------------------------------------------

Navegador: Chrome 90+, Firefox 88+, Safari 14+
JavaScript: Habilitado
LocalStorage: Habilitado
Resolução: 375x667px (mobile) ou DevTools responsivo


----------------------------------------------------------------
Passo 1: Inicializar Sistema
----------------------------------------------------------------
A sua experiencia com este protótipo pode seguir as opções:
A) Caso queira fazer login com personas algum de nossos personas faça:
  Abra seed-database.html no navegador
  Clique em "🌱 Gerar Dados v4.0 HYBRID"
  Aguarde mensagem de sucesso (3 usuários, 10 ativos, 30+ notícias)
  
B) Caso queira fazer um cadastro personalizado para você, faça:
  b.1 Abra index.html(tela6-login.html)
  b.2 clique em "Criar conta grátis" e faça o seu cadatro no app
  b.3 Faça o login utilizando o e-mail e senha cadastrado
  Vá para o Passo 3: "Testar Funcionalidade Principal"
  
  
----------------------------------------------------------------
Passo 2: Fazer Login
----------------------------------------------------------------

Abra index.html(tela6-login.html)
Use uma das credenciais (login /senha):

Iniciante: joaquim@email.com / joaquim123
Investidor: carlos@email.com / carlos123
Analista: beatriz@email.com / beatriz123


----------------------------------------------------------------
Passo 3: Testar Funcionalidade Principal
----------------------------------------------------------------

Uma sequencia de como usar o app:
  - No dashboard, vá para "🔔 Alertas"
  - Clique em "+ Novo"
  - Configure: WEGE3 → Preço → +2.0% → Salvar
  - Abra painel-operador.html em nova aba
  - Selecione WEGE3 → Insira preço 2% maior → Enviar
  - Volte ao dashboard do app → Recarregue (F5) → Veja notificação "NOVO" do ativo WEGE que você cadastrou
  - clique na notificação e seja direcionado para a tela "Notificação", onde podera ter mais detalhes do evento que disparou o alerta.


----------------------------------------------------------------
Estrutura do Projeto
----------------------------------------------------------------
   market-pulse/
   ├── tela1-dashboard.html       # Dashboard principal
   ├── tela2-notificacoes.html    # Gerenciamento de alertas
   ├── tela3-noticias.html        # Feed de notícias
   ├── tela5-historico.html       # Gráficos e análises
   ├── tela6-login.html           # Autenticação
   ├── tela7-perfil.html          # Configurações
   ├── tela8-academy.html         # Conteúdo educacional
   ├── seed-database.html         # EXECUTAR PRIMEIRO
   └── painel-operador.html       # Envio de alertas (admin)


----------------------------------------------------------------
Cenário de Uso: Joaquim, o Iniciante (TUTORIAL DETALHADO DE NAVEGAÇÃO NO APP)
----------------------------------------------------------------

Contexto: Joaquim é técnico eletricista, conhece produtos da WEG, mas nunca investiu por medo.

Roteiro 

1. Aprendendo o Básico (2 min)
- Login: `joaquim@email.com` / `joaquim123`
- Ver badge **"🎓 Iniciante"** e ícones **ℹ️** (tooltips)
- Clicar em **"🎓 Aprender sobre Investimentos"**
- Ler no Glossário: "Ativo", "Volatilidade", "Dividendos"
- Voltar ao dashboard

2. Criando Alerta da WEGE3 (3 min)
- Ir para **"🔔 Alertas"** → **"+ Novo"**
- Selecionar: **WEGE3 - WEG ON**
- Tipo: **📊 Preço**
- Variação: **+2.0%**
- Canais: **WhatsApp + App**
- Clicar em **"Salvar Alerta"**

3. Simulando Variação de Preço (2 min)
- Abrir `painel-operador.html` em nova aba
- Selecionar: **WEGE3**
- Preço atual mostra (ex: R$ 38.50)
- Inserir: **R$ 39.27** (exatamente +2%)
- Clicar em **"📤 Enviar Alerta"**
- Ver confirmação com timestamp

4. Recebendo Notificação (3 min)
- Voltar ao `tela1-dashboard.html`
- **Recarregar página (F5)**
- Ver notificação com badge **"NOVO"**:

  WEGE3
  ▲ +2.0% • R$ 39.27
  Variação de preço atingiu seu alerta

>>> Clicar na notificação
Sistema abre tela5-historico.html com:

Gráfico de 30 dias
Indicadores: SMA 20, SMA 50
Análise: Tendência Altista, Recomendação COMPRA
Sistema de Sentimento: Acurácia 75%

Resultado: O sistema contribui para que o Joaquim entende o básico, ajudando a monitorar 
ativo que conhece e recebe alertas automáticos. Progressivamente pode encorajá-lo a começar a investir.



----------------------------------------------------------------
Checklist de Validação
Funcionalidades Essenciais
----------------------------------------------------------------

   - Sistema de login funcional
   - Criação de alertas (preço e notícias)
   - Envio de alertas pelo operador
   - Notificações com badge "NOVO"
   - Gráficos históricos (Chart.js)
   - Filtros de notícias (impacto, setor, data)
   - Academy com glossário, dicas e quiz
   - Tooltips educacionais para iniciantes
   - Sistema de sentimento com acurácia
