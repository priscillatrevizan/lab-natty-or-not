# Natural ou Fake Natty? Como Vencer na Era das IAs Generativas

## 💡 Apresentação do Projeto
Este projeto documenta, de forma completa, o processo de criação, refinamento e produção de um conteúdo audiovisual educacional utilizando diversas ferramentas de Inteligência Artificial, estimulado pelo desafio `#LabDIONattyOrNot` da [DIO](https://www.linkedin.com/school/dio-makethechange) e prof. [falvojr](https://www.linkedin.com/in/falvojr).

O objetivo foi transformar um conceito técnico — **Chain-of-Thought com Auto-Refinamento** — em uma narrativa simples, coerente e visualmente natural, guiando desde a concepção do roteiro até a geração de prompts detalhados para **lip-sync**, expressões, emoções e continuidade visual.

Além da criação, o projeto registra percepções, caminhos, limitações, prós e contras das ferramentas utilizadas, oferecendo um panorama real sobre o estado atual da produção audiovisual com IA.

---

## 💻 Tecnologias Utilizadas

| Tecnologia | Finalidade |
|-----------|------------|
| **Google Gemini (Flash 2.5)** | Base criativa: concepção da ideia, roteirização, simplificação técnica e estruturação dos prompts. | [Conheça aqui](https://gemini.google.com/) 
| **ElevenLabs** | Geração e refinamento do áudio, ajuste de pausas (...), velocidade e realismo da voz. | [Conheça aqui](https://elevenlabs.io/?utm_source=google&utm_medium=cpc&utm_campaign=brazil_brandsearch_brand_english&utm_id=22349494796&utm_term=elevenlabs&utm_content=brand_-_brand&gad_source=1&gad_campaignid=22349494796&gbraid=0AAAAAp9ksTGQK_GU9AsSL8xL1aE-txALb&gclid=CjwKCAiAw9vIBhBBEiwAraSATnTUCGMA0bxRbxX9kX6TfMdag2Zpu5qA0yEeszwNXojLNtVZlRh9MRoCKk0QAvD_BwE)
| **Perplexity** | Geração de vídeos curtos com alta consistência visual e expressões faciais naturais. | [Conheça aqui](https://studio.d-id.com/video-studio)
| **studio.d-id** | Testes de avatar com importação de áudio (resultados sintéticos ao usar imagens estáticas). | [Conheça aqui](https://studio.d-id.com/video-studio)
| **NotebookLM** | Consolidação de materiais, interligando vídeo, áudio e roteiro para criar resumos em vídeo. | [Conheça aqui](https://notebooklm.google.com/)
| **Veo3 (Google)** | Prova de conceito visual, limitada a 8 segundos por segmento. | [Conheça aqui](https://aistudio.google.com/models/veo-3)
| **Manus** | Ferramenta conceitual para detalhamento frame-by-frame (emoção, ação, postura). | [Conheça aqui](https://manus.im/app)
| **Nano Banana (Google)** | Ferramenta poderosa na criação de imagens com identidade visual. | [Conheça aqui](https://gemini.google/br/overview/image-generation/?hl=pt-BR)

---

## 📝 Processo de Criação

### 1. **Curiosidade inicial → escolha do tema**
Tudo começou com uma pergunta sobre IA. Após análise e refinamento, identifiquei como “macete útil” a técnica de **Chain-of-Thought (CoT) com Auto-Refinamento**.

### 2. **Simplificação narrativa**
Para tornar o conceito acessível, solicitei ao Gemini uma história para crianças de 5 anos explicando a técnica de forma lúdica.

### 3. **Primeiro Roteiro (2:10)**
A história foi transformada em um roteiro detalhado:
- descrição da personagem **Professora Ana**  
- ações naturais (ex: pausa para tomar café)  
- foco em naturalidade e storytelling  

### 4. **Otimização do Tempo**
O roteiro foi reduzido pela metade (aprox. **1:05**) mantendo:
- essência da narrativa  
- clareza da explicação técnica  
- ritmo natural de fala  

### 5. **Quebra em Frames de 8s**
Criado para compatibilidade com ferramentas de vídeo que têm limite curto:
- cada segmento tinha 8 segundos  
- o primeiro frame incluía a definição completa da personagem  

### 6. **Testes Práticos nas Ferramentas**

#### 🔹 *Nano Banana Google*
- qualidade de imagem impressionante  
 cria avatares humanizados de qualidade
Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/imagem_nanobanana.png).

#### 🔹 *Veo3*
- qualidade visual impressionante  
- limite de 8 segundos → inviabiliza continuidade  
- excelente para POCs  
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/video_veo3.mp4).

#### 🔹 *studio.d-id*
- sync labial funcional  
- movimentos sintéticos com imagem estática  
- perde naturalidade  
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/video_id.mp4).

#### 🔹 *Perplexity*
- melhor consistência de cenário  
- expressões faciais humanas e naturais  
- limite de 8 segundos + quota mensal reduzida  
- excelente realismo  
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/video_perplexity.mp4).

#### 🔹 *ElevenLabs*
- áudio altamente natural  
- controle de pausas (...) e velocidade  
- serviu como âncora de timing para todo o projeto  
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/audio_eleven.mp3).

#### 🔹 *Manus*
- ideal para planejamento frame-by-frame  
- garante naturalidade dos movimentos e emoções  
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/roadmap)

#### 🔹 *NotebookLM*
- excelente para consolidar áudio + vídeo + roteiro  
- gera resumos úteis para documentação  
- Gera audios transcritivos sem permissão de ajustes, mas em linguagem natural
- Gera vídeos estilo pitch sem personagens humanos
  Ver [aqui](https://github.com/priscillatrevizan/lab-natty-or-not/blob/main/exemplos/audio_eleven.mp3).
  
### 7. **Criação do Guia Final (Prompt Detalhado)**
Com o áudio final pronto:
- transformei cada trecho em uma instrução detalhada  
- emoções, gestos, postura, direção do olhar  
- foco total em **lip-sync** e **consistência visual da Professora Ana**  
- testei em diversas ferramentas IA de áudio e vídeo

Esse guia funciona como um **prompt universal** para qualquer plataforma de geração de vídeo que permita controle fino ou entrada multimodal.

---

## ✅ Resultados Obtidos

- **Roteiro Hiper-Realista Completo**  
  Pronto para uso em qualquer IA de vídeo moderna.

- **Coerência na Comunicação**  
  O conceito técnico foi traduzido para uma narrativa simples e memorável.

- **Controle Rígido de Tempo**  
  Roteirização modular garantiu o tempo final (1:05).

- **Fidelidade Visual e Sonora**  
  Sincronização labial + gestos + expressão + cenário consistente.

- **Comprovado na prática**  
  Cada ferramenta foi usada até o limite do seu escopo, construindo um pipeline sólido e real.

---

## 🤔 Reflexões e Aprendizados

### Principais limitações encontradas:
- Ferramentas de vídeo com limite curto (8s)
- Movimentos artificiais ao usar avatares estáticos
- Restrições de planos gratuitos (Perplexity, d-id)
- Dificuldade em manter continuidade de cenário entre segmentos separados

### Principais oportunidades:
- Combinação estruturada de ferramentas gera um resultado superior a cada ferramenta isolada.
- A engenharia de prompts torna-se mais importante que a geração de vídeo em si.
- O áudio é o elemento mais estável e confiável do pipeline — deve ser definido primeiro.
- A narrativa modular permite criar vídeos longos usando ferramentas pensadas para clipes curtos.

### Insight mais valioso:
> *Criar vídeos com IA hoje não é apenas gerar vídeo — é engenharia de roteiro, modularização e sincronização precisa. O fluxo começa no áudio, passa pela emoção, e só depois chega ao vídeo.*

---

## 🎥 Conclusão

Este projeto mostrou que, mesmo com limitações importantes nas ferramentas atuais, é possível produzir um conteúdo audiovisual natural, técnico, expressivo e consistente utilizando IA — desde que todo o processo seja guiado por:

- roteirização precisa  
- modularização estratégica  
- engenharia de prompts  
- testes iterativos  

O resultado final é um material profissional, reproduzível e escalável para qualquer criador de conteúdo educacional utilizando Inteligência Artificial.

---

