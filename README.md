# dass_21-Automatizado# Questionário DASS-21 com Áudio e Classificação de Resultados

Este projeto implementa um questionário online baseado no instrumento DASS-21 para avaliação dos níveis de **Depressão**, **Ansiedade** e **Estresse**. Ele inclui funcionalidades para navegação entre perguntas, seleção de respostas, reprodução de áudio associado, validação e exibição de resultados com classificação.

---

## Funcionalidades

- **Perguntas sequenciais**: O usuário responde às perguntas uma a uma.
- **Seleção de respostas**: Quatro opções de resposta (Nunca, Às vezes, Frequentemente, Quase sempre).
- **Reprodução de áudio**: Cada pergunta pode ter um áudio associado, que é reproduzido conforme configuração do usuário.
- **Validação de resposta**: Impede avançar sem selecionar uma resposta, exibindo alerta e tocando áudio.
- **Cálculo de escores**: Soma os pontos das respostas divididas em subescalas para Depressão, Ansiedade e Estresse.
- **Classificação dos escores**: Classifica cada subescala em categorias (Normal, Leve, Moderado, Severo, Extremamente Severo).
- **Exibição dos resultados**: Mostra o nome, idade e resultados finais ao concluir o questionário.

---

## Sobre a Automação do Teste

Este projeto automatiza o questionário DASS-21 utilizando tecnologias web como **HTML**, **JavaScript** e **CSS**, simplificando significativamente a aplicação e análise do teste.

### Benefícios da automação

- **Facilidade de uso:** O teste pode ser aplicado diretamente em navegadores, dispensando formulários em papel ou cálculos manuais.
- **Interatividade:** O usuário responde perguntas sequencialmente, com validações que garantem respostas completas.
- **Feedback imediato:** Os resultados são calculados e exibidos automaticamente após a conclusão do teste, com classificações claras.
- **Acessibilidade:** A reprodução de áudio associada às perguntas facilita o uso para pessoas com dificuldades de leitura.
- **Flexibilidade:** Pode ser facilmente adaptado para diferentes públicos, idiomas e formatos.

Com essa automação, profissionais e pesquisadores podem aplicar o DASS-21 de forma prática e rápida, obtendo resultados confiáveis sem esforço adicional de processamento manual.

---

## Como usar

1. Configure as perguntas, áudios e informações do participante no código (variáveis `questions`, `audios`, `participantName`, `participantAge`).
2. Carregue a página HTML que contém o script.
3. Responda cada pergunta, selecionando uma opção.
4. Se o áudio estiver ativado, ele será reproduzido automaticamente.
5. Após responder todas as perguntas, os resultados serão calculados e exibidos.

---

## Estrutura do código

- `selectAnswer(value)`: Armazena a resposta e exibe o texto selecionado.
- `playAudio()`: Toca o áudio da pergunta atual se o áudio estiver habilitado.
- `showAlertMessage(message)`: Exibe uma mensagem de alerta temporária.
- `nextQuestion()`: Valida resposta, avança para a próxima pergunta ou finaliza o teste.
- `processResponses()`: Calcula escores e classifica os níveis de depressão, ansiedade e estresse.
- Funções `classifyDepression(score)`, `classifyAnxiety(score)`, `classifyStress(score)` para classificar os escores.

---

## Classificação das subescalas

| Subescala | Faixa do Escore          | Classificação           |
|-----------|--------------------------|------------------------|
| Depressão | < 10                     | Normal                 |
|           | 10 - 13                  | Leve                   |
|           | 14 - 20                  | Moderado               |
|           | 21 - 27                  | Severo                 |
|           | > 27                     | Extremamente Severo    |
| Ansiedade | < 8                      | Normal                 |
|           | 8 - 9                    | Leve                   |
|           | 10 - 14                  | Moderado               |
|           | 15 - 19                  | Severo                 |
|           | > 19                     | Extremamente Severo    |
| Estresse  | < 15                     | Normal                 |
|           | 15 - 18                  | Leve                   |
|           | 19 - 25                  | Moderado               |
|           | 26 - 33                  | Severo                 |
|           | > 33                     | Extremamente Severo    |

---

## Dependências

- Navegador com suporte a JavaScript moderno.
- Arquivos de áudio para reprodução (configuráveis no objeto `audios`).
- Estrutura HTML para exibir perguntas, respostas, alertas e resultados.

---

## Possíveis melhorias

- Implementar interface gráfica mais amigável.
- Permitir importar/exportar respostas em CSV.
- Melhorar acessibilidade e suporte a diferentes dispositivos.
- Adicionar suporte multilíngue.

---

## Licença

Este projeto é aberto para uso, modificação e redistribuição.

---

## Contato

Para dúvidas, sugestões ou contribuições, entre em contato.
