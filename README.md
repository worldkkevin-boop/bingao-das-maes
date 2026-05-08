# Bingão das Mães 2026 - Sistema de Sorteio e Telões

Sistema completo e sincronizado em tempo real (via Firebase) para o **Bingão das Mães 2026**. 
Agora o sistema suporta múltiplas telas simultaneamente, permitindo que o operador gerencie o sorteio enquanto o público acompanha em um painel de LED gigante ou nos próprios celulares.

---

## 🚀 Acesso Rápido
**[🎯 Central de Controle Oficial do Bingão](https://worldkkevin-boop.github.io/bingao-das-maes/)**

---

## 📂 Arquivos do Sistema

O sistema é agora composto por 4 arquivos principais:

| Arquivo | Função |
|---------|--------|
| `index.html` | **Painel do Operador:** Interface de controle para marcar os números, gerenciar o prêmio atual e abrir as outras telas. |
| `telao_led.html` | **Tela Principal (Painel LED):** Interface de alto contraste e números gigantes, otimizada para projetores e telões de LED (formato 4x2). |
| `telao.html` | **Tela para Celular:** Versão otimizada (vertical) para o público acompanhar o sorteio no próprio celular. |
| `qrcode.html` | **Tela de QR Code:** Mostra um QR Code gigante para o público escanear e acessar rapidamente o `telao.html`. |

---

## 🎮 Como Usar

### 1. Painel do Operador (`index.html`)
- Acesse a **[Central de Controle Oficial](https://worldkkevin-boop.github.io/bingao-das-maes/)** pelo navegador do computador principal.
- **Gestão de Prêmios:** Clique em "Configurar Prêmios", cole a lista de prêmios a serem sorteados e clique em "Salvar Lista". Clique no nome de um prêmio para destacá-lo no telão.
- **Marcação:** Clique em um número para marcá-lo (ele fica dourado e é enviado em tempo real para os telões).
- **Controles:** Use os botões na parte de baixo para abrir o telão de LED, a tela do celular ou a tela do QR Code.

### 2. Painel LED (`telao_led.html`)
- Abra através do botão "Telão (LED)" no Painel do Operador.
- Arraste a janela para o monitor secundário (o telão de LED).
- Pressione **F11** para colocar em tela cheia. Os elementos se ajustam matematicamente para não criar barras de rolagem.

### 3. Acompanhamento pelo Público (`qrcode.html` e `telao.html`)
- Abra a tela do QR Code (`qrcode.html`) e coloque no telão ou imprima.
- Ao escanear o código, o público acessa o `telao.html` nos próprios celulares, que se atualiza automaticamente sempre que uma nova bola for chamada.

---

## 🎯 Detalhes do Evento

- **Nome**: Bingão das Mães 2026
- **Data**: 09 de Maio de 2026
- **Horário**: 17h00
- **Local**: Terminal Rodoviário
- **Prêmios**: + de R$ 20 mil (PIX, moto, eletrodomésticos)

---

## ⌨️ Atalhos de Teclado

| Atalho | Ação |
|--------|------|
| `F11` | Colocar em tela cheia (funciona em todas as telas) |
| `Ctrl + Z` | Desfazer a última marcação (apenas no Painel do Operador) |
| `ESC` | Sair da tela cheia |

---

## 🔧 Notas e Dicas

- **Internet Obrigatória:** Como o sistema utiliza o banco de dados do Firebase para sincronizar tudo em tempo real, todos os dispositivos precisam de conexão com a internet.
- **Sincronização:** Se alguma tela perder a conexão, basta recarregar a página (F5) para recuperar todo o histórico de bolas chamadas instantaneamente.
- **Link do QR Code:** Certifique-se de que o link dentro do arquivo `qrcode.html` seja o endereço oficial que vai direto para a tela dos celulares: `https://worldkkevin-boop.github.io/bingao-das-maes/telao.html`
