## 🛠️ Guia de Reprodução: Passo a Passo & Prompts

Este guia detalha exatamente como replicar o vídeo **Cyber-Guardian**, desde a geração do texto até a edição final. Copie e cole os prompts nas ferramentas indicadas.

---

## 📝 Fase 1: Roteirização (ChatGPT)

**Ferramenta:** ChatGPT-4 (ou 4o)
**Objetivo:** Criar um roteiro técnico, preciso e cronometrado para 60 segundos.

### 📋 Prompt Exato:
Copie o bloco abaixo e cole no ChatGPT:

```text
Atue como um Instrutor Sênior de Resgate do Corpo de Bombeiros Militar, especialista em PHTLS e Trauma.

Tarefa: Escrever um roteiro para um vídeo curto (Reels/TikTok) de 60 segundos.
Público: Estudantes de primeiros socorros e novos bombeiros.
Cenário: Acidente moto x carro. Motociclista no solo, consciente, com fratura exposta em Tibia/Fíbula e dor na cervical.

Estrutura do Roteiro (Tabela):
1. Tempo (segundos)
2. Falas do Avatar (Tom de voz: Autoritário, calmo e didático)
3. Descrição Visual (O que aparece na tela)

Conteúdo Técnico Obrigatório:
- Segurança da cena (Biossegurança).
- Abordagem XABCDE (foco no X e A).
- Controle de hemorragia na fratura exposta (uso de torniquete ou curativo compressivo conforme protocolo atual).
- Restrição de Movimento da Coluna (RMC) e aplicação do Colar Cervical.

Nota: A linguagem deve ser técnica, mas acessível. Use gírias militares/bombeiro (ex: "QAP", "Padrão", "Na escuta") de forma moderada para gerar conexão.
```
## 🎨 Fase 2: Geração de Imagens (Midjourney / Leonardo AI)

**Ferramenta:** Midjourney v6
**Objetivo:** Criar o cenário de fundo e a base do avatar (caso não use sua própria foto).

### 📸 Prompt 1: O Cenário (Background)
Gera uma rua realista com o acidente, sem mostrar pessoas feridas (para evitar bloqueio da IA), focando no ambiente e iluminação.

```text
Hyper-realistic street level shot, low angle, blurred background of a car crash involving a motorcycle, asphalt texture in focus, sunset dramatic lighting, blue and red emergency lights reflection on the wet wet asphalt, cinematic depth of field, 8k resolution, unreal engine 5 render --ar 9:16 --v 6.0
```

### 📸 Prompt 2: O Avatar (Base do Bombeiro)
Caso você não queira usar uma foto sua, use este prompt para gerar um bombeiro brasileiro com fardamento de combate.

> `Portrait of a Brazilian military firefighter, wearing specific beige/khaki tactical uniform (fardamento de combate a incêndio), looking directly at the camera, neutral but serious facial expression, confident posture, short hair, clean shaven, soft studio lighting, ultra-realistic texture, 8k --ar 9:16 --v 6.0`

*(Dica: Se usar o Leonardo AI, ative o modelo "PhotoReal".)*

## 🗣️ Fase 3: Voz Neural (ElevenLabs)

**Ferramenta:** ElevenLabs
**Objetivo:** Dar vida ao texto com uma voz brasileira natural.

1.  Vá em **"Speech Synthesis"**.
2.  **Configurações de Voz:**
    * **Modelo:** *Eleven Multilingual v2* (Melhor para PT-BR).
    * **Voice Lab:** Escolha uma voz masculina profunda. Sugestões nativas: *"Daniel"* ou *"Clyde"* (ajustado para português).
3.  **Voice Settings (Ajuste Fino):**
    * **Stability:** `50%` (Para permitir variação emocional).
    * **Clarity + Similarity Enhancement:** `75%` (Para garantir dicção perfeita dos termos técnicos).
4.  Cole o texto da coluna "Falas do Avatar" gerada pelo ChatGPT e faça o download do MP3.

## 🎭 Fase 4: Animação do Avatar (HeyGen)

**Ferramenta:** HeyGen (ou D-ID como alternativa)
**Objetivo:** Sincronizar a imagem do bombeiro com o áudio.

1.  Crie um **"Photo Avatar"**.
2.  Faça upload da imagem do Bombeiro gerada no Midjourney (ou sua foto).
3.  Faça upload do áudio (MP3) gerado no ElevenLabs.
4.  Clique em **"Submit"** para gerar o vídeo do personagem falando.
5.  **Dica:** Escolha "Transparent Background" (se disponível no plano) ou fundo verde (Green Screen) para facilitar a edição no CapCut.

## 🎬 Fase 5: Edição e Montagem (CapCut)

**Ferramenta:** CapCut (PC ou Mobile)
**Objetivo:** Unir tudo e dar o estilo "Aesthetic".

1.  **Camada 1 (Fundo):** Coloque a imagem do cenário (Prompt 1).
2.  **Camada 2 (Avatar):** Coloque o vídeo do HeyGen. Remova o fundo (Recorte Inteligente ou Chroma Key) e posicione o bombeiro na parte inferior central.
3.  **Camada 3 (Overlays):**
    * Busque em bancos de imagem (ou gere) imagens de "Fratura Exposta Ilustrativa" ou use stickers do CapCut para simular o ferimento (cuidado com as regras de violência das redes sociais).
    * Adicione setas apontando para a perna e para o pescoço quando o áudio falar sobre eles.
4.  **Legendas:** Use a função **"Legendas Automáticas"**. Escolha uma fonte bold e moderna (Ex: *Montserrat* ou *The Bold Font*). Use cores vibrantes (Amarelo ou Vermelho) para palavras-chave (Ex: **Torniquete**, **RMC**).
5.  **Áudio:** Adicione um som de "Siren Ambience" (sirene distante) em volume baixo (10-15%) para compor a atmosfera.

---

## ⚠️ Nota Ética
Todo o conteúdo gerado deve passar por revisão técnica humana. IAs podem alucinar protocolos. Como bombeiro, **sempre valide** se a instrução do roteiro bate com o POP (Procedimento Operacional Padrão) da sua corporação (CBMMS) antes de publicar.
