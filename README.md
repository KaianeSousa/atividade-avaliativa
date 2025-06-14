# atividade-avaliativa

# 💅 L’Unha - Estúdio

Site institucional desenvolvido para o **L’Unha - Estúdio**, com foco na apresentação dos serviços, agendamento online e acessibilidade. O projeto utiliza **HTML**, **CSS com Bootstrap 5** e **JavaScript puro**, prezando por uma experiência leve, responsiva e acolhedora ao público-alvo.

---

## 📌 Tema e Estrutura da Página

O site foi pensado para um **estúdio de unhas** moderno e feminino, com navegação intuitiva. A estrutura está organizada em seções:

- **Banner principal** com mensagem de boas-vindas dinâmica
- **Compromissos** do estúdio com os clientes
- **Serviços oferecidos** com detalhes condicionais
- **Formulário de agendamento** interativo
- **Rodapé** com redes sociais e botão de troca de tema (claro/escuro)

---

## 🎨 Justificativa do Design

### Cores
- Utilizamos tons claros e escuros com contraste suficiente para atender critérios de **acessibilidade visual**.
- O site tem **modo claro** por padrão, com opção para modo escuro via botão toggle.
- O fundo da seção de serviços usa um tom **pastel suave**, transmitindo leveza e sofisticação.

### Fontes
- A tipografia foca em **clareza e elegância**, usando famílias sans-serif combinadas com peso variado para títulos e conteúdo.

### Responsividade
- Com base no **Bootstrap 5**, o layout adapta-se bem a diferentes tamanhos de tela.
- Elementos ocultos/mostrados conforme a resolução e suporte a **JavaScript**.
- Menu, formulário e seções garantem acessibilidade e usabilidade em dispositivos móveis.

---

## ⚙️ Funcionalidades em JavaScript

O site tem diversas funcionalidades implementadas com JavaScript puro:

### ✅ Detecção de horário e saudação automática
```js
function mostrarMensagemHorario() {
  const hora = new Date().getHours();
  let mensagem = '';

  if (hora >= 5 && hora < 12) {
    mensagem = 'Bom dia! Bem-vinda ao Unha Pop Estúdio, estamos funcionando';
  } else if (hora >= 12 && hora < 18) {
    mensagem = 'Boa tarde! Pronta para renovar suas unhas?';
  } else {
    mensagem = 'Boa noite! Horário perfeito para pensar em cuidar de você';
  }

  // Exibe a mensagem antes do título no banner
}
