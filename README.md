# Bingão das Mães 2026 - Sistema de Marcação + Telão

Sistema completo com **duas telas** para o Bingão das Mães 2026:
- **Tela do operador** (`index.html`) — para marcar os números sorteados no notebook
- **Tela do telão** (`telao.html`) — para o público ver os números que já saíram, bem grandão

As duas telas se sincronizam automaticamente via `localStorage`.

---

## 🎮 Como Usar

### 1. Tela do Operador (notebook)
- Abra `index.html` no navegador
- Clique no número sorteado para **marcar** (fica dourado)
- Clique novamente no mesmo número para **desmarcar**
- **"Resetar"** limpa tudo (com confirmação)
- **"Desfazer"** remove a última marcação
- **"Abrir Telão"** abre a tela do telão em nova aba
- **"Tela Cheia"** (F11) ocupa 100% da tela

### 2. Tela do Telão (projetor)
- Abra `telao.html` no navegador
- Deixe em **Tela Cheia** (F11)
- Arraste para o monitor do projetor (se tiver 2 monitores)
- Os números aparecem automaticamente quando o operador marca!
- O **último número sorteado** fica enorme e piscando no topo
- Todos os números já sorteados ficam em dourado no grid

---

## 📂 Arquivos

| Arquivo | Função |
|---------|--------|
| `index.html` | Tela de marcação do operador (75 números em grid 5 colunas) |
| `telao.html` | Tela do telão (último número grande + grid dos sorteados) |

---

## 🎯 Evento

- **Nome**: Bingão das Mães 2026
- **Data**: 09 de Maio de 2026
- **Horário**: 17h
- **Local**: Terminal Rodoviário
- **Prêmios**: + de R$ 20 mil (PIX, moto, eletrodomésticos)

---

## ⌨️ Atalhos do Teclado

| Atalho | Ação |
|--------|------|
| `F11` | Tela cheia |
| `Ctrl + Z` | Desfazer última marcação |
| `ESC` | Sair da tela cheia |

---

## 🔧 Dicas

- **Monitor duplo**: Abra `index.html` no notebook e `telao.html` no projetor
- **Funciona offline**: Tudo é local, não precisa de internet
- **Sincronização automática**: Quando o operador clica, o telão atualiza na hora
- **Se não sincronizar**: Recarregue a página do telão (F5)
