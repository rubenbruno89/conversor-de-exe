# File Smuggling Builder

## Descrição
O **File Smuggling Builder** é uma ferramenta em HTML e JavaScript que permite incorporar arquivos como texto codificado em um novo arquivo HTML. Com uma camada de segurança básica, ele utiliza uma senha de XOR para codificar o conteúdo do arquivo. Após gerar o arquivo HTML, o usuário pode baixar e recuperar o arquivo original a partir do HTML criado.

## Funcionalidades
- **Incorporação de Arquivos**: Carrega e converte qualquer arquivo em uma string codificada Base64, incorporada em HTML.
- **Proteção por Senha**: Utiliza uma codificação XOR com senha definida pelo usuário para proteger o conteúdo do arquivo.
- **Geração de HTML**: Cria um novo arquivo HTML que pode armazenar o arquivo original, permitindo download e recuperação.
- **Compatibilidade com Blob**: Utiliza a API Blob para criar objetos de download e manipulação de arquivos.

## Estrutura do Projeto
- **HTML/CSS**: Interface simples para seleção de arquivo, definição de senha e mensagem personalizada.
- **JavaScript**: Scripts para codificar o arquivo em Base64, aplicar XOR com senha, e gerar o HTML incorporado.

## Como Usar
1. Abra o arquivo `index.html` no navegador.
2. No menu da interface, selecione o arquivo desejado em **"Choose file"**.
3. Insira uma senha em **"Set open password"** para proteger o arquivo.
4. Opcionalmente, adicione uma mensagem personalizada no campo **"Message"**.
5. Clique em **"Build Embedded HTML file"** para gerar o arquivo HTML.
6. Um novo arquivo HTML será baixado automaticamente. Este arquivo pode ser aberto em um navegador para visualizar e recuperar o arquivo original.

## Estrutura do Código
- **Função `build()`**: Lê o arquivo selecionado e o converte para Base64.
- **Função `xor()`**: Aplica a codificação XOR usando a senha fornecida.
- **Função `generatehtml()`**: Cria o HTML com o conteúdo Base64 e fornece a opção de recuperação do arquivo.

## Licença
Este projeto está licenciado sob a licença MIT.

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request para melhorias ou correções.
