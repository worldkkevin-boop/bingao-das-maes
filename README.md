# Bingão das Mães 2026 - Sistema de Sorteio e Telões

Sistema completo e sincronizado em tempo real (via Firebase) para o **Bingão das Mães 2026**. 
Agora o sistema suporta múltiplos ecrãs em simultâneo, permitindo que o operador gira o sorteio enquanto o público acompanha num painel de LED gigante ou nos seus próprios telemóveis.

---

## 📂 Ficheiros do Sistema

O sistema é agora composto por 4 ficheiros principais:

| Ficheiro | Função |
|---------|--------|
| `index.html` | **Painel do Operador:** Interface de controlo para marcar os números, gerir o prémio atual e abrir os outros ecrãs. |
| `telao_led.html` | **Ecrã Principal (Painel LED):** Interface de alto contraste e números gigantes, otimizada para projetores e painéis de LED (formato 4x2). |
| `telao.html` | **Ecrã para Telemóvel:** Versão otimizada (vertical) para o público acompanhar o sorteio no próprio telemóvel. |
| `qrcode.html` | **Ecrã de QR Code:** Mostra um QR Code gigante para o público ler e aceder rapidamente ao `telao.html`. |

---

## 🎮 Como Usar

### 1. Painel do Operador (`index.html`)
- Abra o `index.html` no navegador do computador principal.
- **Gestão de Prémios:** Clique em "Configurar Prémios", cole a lista de prémios a sortear e clique em "Salvar Lista". Clique num prémio para o destacar nos ecrãs.
- **Marcação:** Clique num número para o marcar (fica dourado e é enviado para os ecrãs).
- **Controlos:** Use os botões na base para abrir o ecrã LED, o ecrã do telemóvel ou o QR Code diretamente do painel.

### 2. Painel LED (`telao_led.html`)
- Abra através do botão verde no Painel do Operador.
- Arraste a janela para o monitor secundário (o painel de LED).
- Pressione **F11** para colocar em ecrã inteiro. Os elementos ajustam-se automaticamente para não criar barras de rolagem.

### 3. Acompanhamento pelo Público (`qrcode.html` e `telao.html`)
- Abra o ecrã do QR Code (`qrcode.html`) e mostre ao público (ou imprima).
- Ao ler o código, o público acede ao `telao.html` nos seus telemóveis, atualizando automaticamente sempre que uma bola é chamada.

---

## 🎯 Detalhes do Evento

- **Nome**: Bingão das Mães 2026
- **Data**: 09 de Maio de 2026
- **Horário**: 17h00
- **Local**: Terminal Rodoviário
- **Prémios**: + de R$ 20 mil (PIX, moto, eletrodomésticos)

---

## ⌨️ Atalhos de Teclado

| Atalho | Ação |
|--------|------|
| `F11` | Colocar em ecrã inteiro (funciona em todos os ecrãs) |
| `Ctrl + Z` | Desfazer a última marcação (apenas no Operador) |
| `ESC` | Sair do ecrã inteiro |

---

## 🔧 Notas e Dicas

- **Internet Obrigatória:** Como o sistema agora utiliza a base de dados em tempo real do Firebase para sincronizar tudo instantaneamente, todos os dispositivos precisam de ligação à internet.
- **Sincronização:** Se um ecrã perder a ligação, basta recarregar a página (F5) para recuperar todo o histórico atualizado.
- **Hospedagem:** Certifique-se de que substituiu o link padrão no ficheiro `qrcode.html` pelo link real onde os ficheiros do seu bingo estão alojados.
