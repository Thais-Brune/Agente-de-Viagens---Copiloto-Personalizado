# Agente-de-Viagens---Copiloto-Personalizado

## Desafio

Criar um Copiloto com fluxo de conversa personalizado usando o **Microsoft Copilot Studio**, simulando um atendimento de um agente de viagens.

Este projeto faz parte de um desafio prático que visa aplicar a criação de copilotos com inteligência artificial generativa, usando fluxos de conversa estruturados e personalizados.

---

## O que foi aprendido

Durante o desenvolvimento do desafio, foram adquiridas as seguintes habilidades:

- Criar um copiloto com base em fluxos personalizados no **Copilot Studio**.
- Utilizar **frases de gatilho** para identificar intenções do usuário.
- Construir **condições e caminhos lógicos** de diálogo com base em preferências.
- **Coletar dados do usuário** e armazenar em variáveis.
- Testar, publicar e compartilhar copilotos funcionais.
- Pensar em **experiências reais de atendimento** automatizado.

---

## Passo a Passo Técnico para Criar o Copiloto (Agente de Viagens)

### 1. Acessar o Microsoft Copilot Studio

- Acesse: [https://copilotstudio.microsoft.com/](https://copilotstudio.microsoft.com/)
- Faça login com sua conta Microsoft.

---

### 2. Criar um Novo Copiloto

1. Clique em **"Copilotos"** no menu lateral.
2. Clique em **“+ Novo copiloto”**.
3. Dê um nome ao copiloto (ex: `AgenteDeViagensAI`).
4. Selecione o idioma: **Português (Brasil)**.
5. Clique em **"Criar"**.

---

### 3. Configurar Saudação Inicial

1. Vá até a aba **Tópicos**.
2. Selecione o tópico **Saudação (Greeting)**.
3. Edite a mensagem de boas-vindas:

```text
Olá! Eu sou seu assistente de viagens virtual. Posso ajudar com sugestões de destinos, pacotes, passagens ou hospedagens. O que você gostaria de saber hoje?

### 4. Criar Tópico Personalizado: "Sugestão de Viagem"
Clique em "Novo tópico".

Nomeie como SugestaoDeViagem.

No campo Frases de gatilho, adicione:

Quero viajar
Me indique um destino
Sugestão de lugar para férias
Estou planejando uma viagem

### 5.Estrutura Geral do Fluxo

1. Saudação inicial
2. Identificação da intenção do usuário
3. Perguntas direcionadas (com opções)
4. Respostas baseadas em condições
5. Coleta de dados para contato ou envio de pacotes
6. Encerramento amigável ou redirecionamento

### 6. Exemplo de Diálogo Esperado

Usuário: Quero viajar
Copiloto: Que ótimo! Você tem um tipo de destino em mente? (praia, montanha, cidade, natureza)
Usuário: Praia
Copiloto: Maravilha! Temos pacotes incríveis para Maragogi, Jericoacoara e Fernando de Noronha. Qual deles mais te interessa?
Usuário: Fernando de Noronha
Copiloto: Excelente escolha! Gostaria de receber detalhes por e-mail?
Usuário: Sim
Copiloto: Perfeito. Por favor, informe seu nome e e-mail para enviarmos as opções disponíveis.

### 7. Lógica de Decisão (Condicionais)
O fluxo utiliza condições de resposta para ramificar o atendimento com base na escolha do usuário.

Exemplo:
Se resposta contém "praia" ➝ Sugerir destinos com praia
Se resposta contém "montanha" ➝ Sugerir destinos frios ou com altitude
Se resposta contém "aventura" ➝ Sugerir ecoturismo
Se resposta não reconhecida ➝ Pedir para repetir ou sugerir opções

### 8. Teste o copiloto e depois publique.


