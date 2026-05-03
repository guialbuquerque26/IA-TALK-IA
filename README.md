# IA-TALK-IA

Um projeto em Python que promove uma conversa autônoma entre duas Inteligências Artificiais: **Google Gemini** e **Cohere**. 

## Descrição

O script `IAtalks.py` solicita um tema ao usuário e inicia um diálogo entre os modelos de IA, onde um responde ao outro em um loop de turnos definidos. Ao final da interação, o sistema solicita ao Gemini que elabore um relatório detalhado da conversa, salvando-o automaticamente em um arquivo de texto (`resumo_conversa.txt`) dentro de uma pasta com o nome do tema discutido.

## Pré-requisitos

Certifique-se de ter o Python instalado na sua máquina (recomendado Python 3.8 ou superior).

Instale as dependências necessárias executando o seguinte comando:

```bash
pip install google-generativeai cohere python-dotenv
```

## Configuração

1. Clone ou baixe este repositório.
2. Crie um arquivo `.env` na raiz do projeto contendo as suas chaves de API:

```env
GEMINI_API_KEY=sua_chave_aqui
COHERE_API_KEY=sua_chave_aqui
```

> **Nota:** As credenciais foram movidas para o arquivo `.env` para garantir a segurança. Este arquivo está sendo ignorado pelo `.gitignore` e não será comitado no seu repositório.

## Como Executar

Execute o script principal via terminal:

```bash
python IAtalks.py
```

1. O script solicitará um tema.
2. Você acompanhará a conversa no terminal em tempo real.
3. Ao final de 5 turnos, será gerado um relatório salvo na pasta correspondente ao tema.

## Funcionalidades
- Integração com **Google Gemini** (`gemini-2.0-flash`) e **Cohere** (`command`).
- Geração automática de relatórios resumidos com análises usando a própria IA.
- Organização automática de arquivos de saída em diretórios nomeados dinamicamente.