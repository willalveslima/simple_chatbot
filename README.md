
# Projeto de Chatbot Simples com Deep Learning

Este projeto utiliza a Deep Learning para criar um chatbot Simples. Ele inclui dois scripts principais:   `treino_do_modelo.py` e  `chat.py` .
Referência: Artigo  [How To Build Your Own Chatbot Using Deep Learning](https://https://towardsdatascience.com/how-to-build-your-own-chatbot-using-deep-learning-bb41f970e281)

## Índice

- [Instalação](#instalação)
- [Uso](#uso)
  - [Treinamento do Modelo](#treinamento-do-modelo)
  - [Chatbot](#chatbot)
  
- [Requisitos](#requisitos)
- [Licença](#licença)

## Instalação

1. Clone o repositório:
    ```sh
    git clone https://github.com/willalveslima/simple_chatbot.git
    cd seu-repositorio
    ```

2. Crie e ative um ambiente virtual:
    ```sh
    python -m venv venv
    source venv/bin/activate  # No Windows use `venv\Scripts\activate`
    ```

3. Instale as dependências:
    ```sh
    pip install openai
    ```

4. Adicione sua chave de API do OpenAI no arquivo `chave_api.txt`.

## Uso



### Treinamento do Modelo

O script `treino_do_modelo.py` permite realizar o treinamento do modelo com dados dos tokens.

1. Prepare seu arquivo de dados de treino no formato JSON e salve-o como `intents.jsonl`.

2. Execute o script:
    ```sh
    python treino_do_modelo.py
    ```

### Chatbot

O script `chat.py` permite que você faça a interação com o modelo e receba respostas.

1. Execute o script:
    ```sh
    python chat.py
    ```

Exemplo de interação:

```sh
   Start messaging with the bot (type quit to stop)!
User: Hi 
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 55ms/step
ChatBot: Hello
User: I need help
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 15ms/step
ChatBot: Tell me how can assist you
User: install software
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 14ms/step
ChatBot: Hi
User: olá
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 14ms/step
ChatBot: Hi there
User: what is your name?
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 14ms/step
ChatBot: You can call me Joana.
User: hi joana
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 16ms/step
ChatBot: Hi
User: by
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 13ms/step
ChatBot: Hello
User: quit
```


## Requisitos

colorama==0.4.6
keras==3.4.1
numpy==1.26.4
scikit-learn==1.5.1
tensorflow==2.17.0



## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
