# Proposta Inicial do Jogo

## 1. Nome provisório do jogo

**Nome:**

> Não Compartilhe!

## 2. Integrantes do grupo

- Nome 1: Carlos Eduardo
- Nome 2: Augusto Zagnoli

## 3. Tema escolhido

**Tema:**

> Privacidade e proteção de dados: compartilhamento responsável de informações pessoais com assistentes virtuais e aplicativos de IA (eixo: Inteligência Artificial no Cotidiano: Aplicações e Uso Responsável).
>
> **Relevância:** assistentes e chatbots de IA já fazem parte do dia a dia. As pessoas pedem ajuda com tarefas, colam textos, enviam fotos e documentos, muitas vezes sem pensar que o conteúdo enviado pode ficar armazenado nos servidores da empresa, ser revisado por terceiros ou ficar exposto em um vazamento. Saber o que pode e o que não pode ser compartilhado é parte essencial do uso responsável da IA.

**Como esse tema se relaciona com o jogo?**

> O tema define a regra central. O celular do jogador representa um aplicativo de assistente de IA, e cada cartão que cai é algo que o usuário poderia enviar a ele. O jogador precisa ler e decidir: pegar (compartilhar) ou deixar passar. Informações seguras dão pontos; dados sensíveis (senha, CPF, foto de documento) custam uma vida e mostram por que não devem ser compartilhados. Todos os cartões têm a mesma cor, então a decisão depende de entender o conteúdo.

## 4. Tipo de jogo

**Tipo escolhido:**

> Coleta e desvio de itens (cartões caindo do topo da tela).

## 5. Descrição geral do jogo

**Descrição:**

> A tela mostra, na parte inferior, um celular com o aplicativo "Assistente IA", controlado pelo jogador. Do topo caem cartões de texto em posições aleatórias, cada um com um texto curto, como "Receita de bolo", "Dúvida de física", "Senha do banco" ou "Foto do RG". Na parte de cima da tela aparecem os pontos, as vidas e o tempo restante. Quando o jogador pega um dado sensível, aparece por alguns segundos uma mensagem curta explicando o risco (por exemplo: "Senhas nunca devem ser enviadas a um chatbot"). Com o passar do tempo, os cartões caem mais rápido, exigindo leitura e decisão cada vez mais rápidas.

## 6. Objetivo do jogador

**Objetivo:**

> Chegar ao fim dos 60 segundos da partida com o máximo de pontos, pegando apenas informações seguras e deixando os dados sensíveis passarem.

## 7. Regras principais

- Regra 1: O jogador move o celular para a esquerda e para a direita e começa com 3 vidas.
- Regra 2: Pegar um cartão com informação segura soma 10 pontos.
- Regra 3: Pegar um cartão com dado sensível tira 1 vida e mostra o motivo pelo qual aquele dado não deve ser compartilhado.
- Regra 4: Cartões que chegam ao fim da tela sem serem pegos desaparecem sem alterar pontos ou vidas.
- Regra 5: A cada 15 segundos, a velocidade de queda dos cartões aumenta.

## 8. Condição de vitória

**Condição de vitória:**

> Chegar ao fim dos 60 segundos com pelo menos 1 vida. A tela final mostra a mensagem "Seus dados estão seguros!" e a pontuação obtida.

## 9. Condição de derrota ou encerramento

**Condição de derrota ou encerramento:**

> O jogador perde quando as 3 vidas acabam antes do fim do tempo, e a tela final mostra "Seus dados vazaram!". Em qualquer final, a pontuação é comparada com o ranking e, se estiver entre as 5 maiores, é salva. Na tela final, o jogador pode jogar de novo (ENTER) ou sair (ESC). A partida também pode ser encerrada a qualquer momento com ESC.

## 10. Elementos previstos no jogo

- **Personagem ou elemento principal:** celular com o aplicativo "Assistente IA" (retângulo desenhado com Pygame ou imagem simples), controlado pelo jogador na parte inferior da tela.
- **Obstáculos ou desafios:** cartões com dados sensíveis, por exemplo: "Senha do banco", "CPF", "Foto do RG", "Número do cartão", "Endereço de casa".
- **Itens ou objetos de interação (se houver):** cartões com informações seguras de compartilhar, por exemplo: "Receita de bolo", "Dúvida de física", "Ideia de presente", "Resumo de um texto", "Plano de estudos".
- **Pontuação, vidas, tempo ou progresso:** pontos (+10 por item seguro), 3 vidas, cronômetro de 60 segundos e ranking com as 5 maiores pontuações, salvo em arquivo.

## 11. Controles previstos

**Controles:**

> Setas ← / → (ou A / D) para mover o celular; ENTER para começar a partida ou jogar de novo; ESC para sair do jogo.

## 12. Principais dificuldades esperadas

- Dificuldade 1: Mostrar o texto dentro dos cartões de forma legível enquanto eles estão em movimento.
- Dificuldade 2: Equilibrar a velocidade e a quantidade de cartões para o jogo não ficar fácil nem difícil demais.
- Dificuldade 3: Ler e salvar os arquivos (cartões e ranking) sem erros, inclusive quando o arquivo de ranking ainda não existir.

## 13. Escopo mínimo para a entrega final

**Escopo mínimo:**

> Tela inicial com o nome do jogo e as instruções; tela de jogo com o celular controlado pelo teclado; cartões caindo, com textos lidos do arquivo `data/itens.csv`; colisão entre o celular e os cartões, aplicando as regras de pontos e vidas; mensagem com o motivo ao pegar um dado sensível; pontos, vidas e tempo exibidos na tela; tela final de vitória ou derrota; ranking com as 5 maiores pontuações salvo em `data/ranking.txt`; testes com pytest para as funções de lógica do jogo.

## 14. Possíveis melhorias, caso haja tempo

- Melhoria 1: Tela final com o resumo dos dados sensíveis que o jogador "vazou" na partida (usando um conjunto, sem repetição) e uma dica para cada um.
- Melhoria 2: Digitar o nome do jogador para aparecer no ranking.
- Melhoria 3: Sons ao pegar cartões e imagens simples para o celular e o fundo.

---

## Seções complementares (itens pedidos no enunciado do Canvas)

## 15. Aspecto de uso responsável e integração com a jogabilidade

**Aspecto de uso responsável:** privacidade e proteção de dados. Ao usar um assistente de IA, o próprio usuário decide o que compartilha e é responsável por proteger seus dados pessoais.

**Integração com a jogabilidade:**

- A regra de pontos e vidas depende diretamente de o cartão conter um dado seguro ou sensível.
- Todos os cartões têm a mesma cor: o jogador só acerta se ler e entender o conteúdo.
- Ao errar, o jogador vê o motivo do risco, o que transforma cada erro em aprendizado.
- Não há IA real no jogo. A classificação de cada cartão (seguro ou sensível) é definida no arquivo de dados e tratada com condicionais e dicionários, simulando um "filtro de privacidade".

## 16. Estruturas de dados previstas

- **Dicionário** para cada cartão:
  `{"texto": "Senha do banco", "sensivel": True, "motivo": "Senhas nunca devem ser enviadas a um chatbot", "x": 120, "y": -40}`
- **Lista** com os cartões que estão caindo na tela.
- **Lista** com os modelos de cartões lidos do arquivo, sorteados com `random.choice`.
- **Dicionário** com o estado da partida: `{"pontos": 0, "vidas": 3, "tempo": 60, "velocidade": 3}`.
- **Tuplas** para as cores (RGB) e o tamanho da tela.
- **Lista** de inteiros para o ranking, ordenada e limitada a 5 posições.

## 17. Uso de arquivos

- **`data/itens.csv` (leitura):** lido no início do jogo. Cada linha tem o texto do cartão, se ele é sensível e o motivo. Assim, é possível adicionar novos cartões sem mexer no código. Exemplo:

  ```
  texto;sensivel;motivo
  Receita de bolo;nao;
  Dúvida de física;nao;
  Senha do banco;sim;Senhas nunca devem ser enviadas a um chatbot
  CPF;sim;O CPF pode ser usado em golpes e fraudes
  Foto do RG;sim;Documentos com foto permitem que alguém se passe por você
  ```

- **`data/ranking.txt` (leitura e escrita):** guarda as 5 maiores pontuações, uma por linha. É lido no início e atualizado ao final de cada partida. Se o arquivo não existir, o jogo começa com o ranking vazio e cria o arquivo.

## 18. Organização inicial do código

O projeto seguirá a estrutura do template da disciplina (`main.py`, `src/`, `data/`, `tests/`, `assets/`, `docs/`). Os nomes dos módulos abaixo poderão ser adaptados aos arquivos que já existem no template.

```
main.py              → ponto de entrada; chama a função principal do jogo
src/config.py        → constantes (tamanho da tela, cores, velocidade, tempo)
src/regras.py        → funções de lógica sem Pygame (pontos, vidas, vitória/derrota, ranking)
src/cartoes.py       → criar, mover e desenhar cartões; verificar colisão
src/arquivos.py      → ler itens.csv; ler e salvar ranking.txt
src/jogo.py          → loop principal e telas (início, jogo, fim)
data/itens.csv       → cartões do jogo
data/ranking.txt     → ranking das maiores pontuações
tests/test_regras.py
tests/test_arquivos.py
```

As regras ficam separadas do código do Pygame (`src/regras.py`), o que facilita testar a lógica sem abrir a janela do jogo.

**Divisão prevista do trabalho:**

| Integrante | Responsabilidade principal |
|---|---|
| Carlos Eduardo | Loop principal e telas (`jogo.py`, `main.py`) e cartões: criação, movimento, desenho e colisão (`cartoes.py`) |
| Augusto Zagnoli | Regras e testes (`regras.py`, `tests/`) e arquivos e dados (`arquivos.py`, `itens.csv`, `ranking.txt`) |
| Ambos | README.md, revisão do código e apresentação |

## 19. Testes planejados

Testes simples com pytest para as funções de lógica:

| Função | O que será testado |
|---|---|
| `eh_sensivel(cartao)` | Retorna `True` para "CPF" e `False` para "Receita de bolo" |
| `calcular_pontos(pontos, cartao)` | Soma 10 com item seguro; não altera com dado sensível |
| `atualizar_vidas(vidas, cartao)` | Tira 1 vida com dado sensível; não altera com item seguro |
| `verificar_fim(vidas, tempo)` | Retorna `"derrota"` com 0 vidas, `"vitoria"` com tempo esgotado e vidas restantes, e `None` durante a partida |
| `calcular_velocidade(tempo_decorrido)` | A velocidade aumenta a cada 15 segundos |
| `atualizar_ranking(ranking, pontos)` | Mantém a lista ordenada do maior para o menor, com no máximo 5 pontuações |
| `ler_itens(caminho)` | Lê um arquivo de teste e retorna uma lista de dicionários com texto, sensível (booleano) e motivo |

## 20. Recursos previstos

- Python 3 e Pygame (desenvolvimento do jogo).
- pytest (testes).
- Fonte padrão do Pygame e formas desenhadas com `pygame.draw` (sem imagens externas no escopo mínimo).
- Template oficial da disciplina: https://github.com/ICEI-PUC-Minas-PPL-CDIA/IntroAlgs_pygame_template
- Assistente de IA (Claude), usado como apoio na organização das ideias desta proposta. O código será escrito, revisado e explicado pelos integrantes do grupo.
- Qualquer imagem, som, fonte ou trecho de código externo adicionado depois será citado no README.md, com origem e, quando possível, licença.

## 21. Declaração de originalidade

Declaramos que o jogo "Não Compartilhe!" é uma proposta autoral do grupo, desenvolvida a partir do template oficial da disciplina. O jogo não reutiliza projetos de semestres anteriores e não é cópia de tutoriais, repositórios ou exemplos prontos. Todo recurso externo utilizado (código, imagens, sons, fontes ou tutoriais) será identificado no README.md com sua origem e, quando possível, sua licença.
