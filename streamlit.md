### Passos para Configurar Ambiente Virtual Python e Streamlit no Windows, macOS e Linux

1. **Instalar Python (se ainda não instalado)**:
   - **Windows**: Baixe e instale o Python: https://www.python.org/downloads/
   - **macOS/Linux**: Python já vem pré-instalado na maioria dos sistemas. Para verificar, use:
     ```bash
     python3 --version
     ```
   - Verifique a instalação:
     - **Windows**: Abra o Prompt de Comando (cmd) e digite:
       ```bash
       python --version
       ```
     - **macOS/Linux**: Abra o terminal e digite:
       ```bash
       python3 --version
       ```

2. **Criar o Ambiente Virtual (venv)**:
   - **Windows**:
     - Abra o **Prompt de Comando** e navegue até a pasta do projeto ou crie uma nova pasta:
       ```bash
       mkdir meu_projeto
       cd meu_projeto
       ```
     - Crie o ambiente virtual:
       ```bash
       python -m venv venv
       ```
     - Ative o ambiente virtual:
       ```bash
       venv\Scripts\activate
       ```
   - **macOS/Linux**:
     - Abra o terminal e navegue até a pasta do projeto ou crie uma nova pasta:
       ```bash
       mkdir meu_projeto
       cd meu_projeto
       ```
     - Crie o ambiente virtual:
       ```bash
       python3 -m venv venv
       ```
     - Ative o ambiente virtual:
       ```bash
       source venv/bin/activate
       ```

3. **Instalar o Streamlit**:
   - Com o ambiente virtual ativo, instale o Streamlit:
     ```bash
     pip install streamlit
     ```

4. **Criar o arquivo `example.py`**:
   - Crie um arquivo `example.py` com o seguinte código:
     ```python
     import streamlit as st

     st.title("Hello, Streamlit!")
     st.write("Este é um exemplo simples de uma aplicação Streamlit.")

     nome = st.text_input("Digite seu nome:")
     if nome:
         st.write(f"Olá, {nome}!")
     ```
   - Salve o arquivo no diretório do seu projeto.

5. **Rodar o Streamlit**:
   - Execute o comando para rodar o Streamlit:
     ```bash
     streamlit run example.py
     ```
   - Isso abrirá o navegador com sua aplicação rodando!

6. **Desativar o Ambiente Virtual**:
   - Após terminar, desative o ambiente virtual:
     ```bash
     deactivate
     ```

Pronto! Seu ambiente virtual está configurado e o exemplo Streamlit funcionando.
