# 🎬 ClipMaker - NLW Connect

O **ClipMaker** é uma aplicação web desenvolvida durante o evento NLW (Next Level Week) da Rocketseat. O objetivo do projeto é permitir o upload de vídeos ou áudios e, através da integração com o Cloudinary, obter a transcrição automática do conteúdo e identificar "momentos virais".

## ✨ Funcionalidades

*   **Upload Inteligente:** Integração com o Cloudinary Upload Widget para envio de arquivos na nuvem.
*   **Transcrição Automática:** Captura arquivos `.transcript` gerados após o processamento do vídeo.
*   **Detecção de Momentos:** Algoritmo simples para filtrar palavras-chave (como "viral", "moment", "boom") na transcrição e identificar pontos altos do vídeo.
*   **Interface Minimalista:** Exibição em tempo real do progresso e do JSON resultante no navegador.

## 🚀 Tecnologias Utilizadas

*   **HTML5/CSS3**: Estrutura e estilização básica.
*   **JavaScript (Vanilla)**: Lógica de polling, integração com API e manipulação de DOM.
*   **[Cloudinary](https://cloudinary.com/):** Serviço de hospedagem e processamento de mídia (IA de transcrição).

## 🛠️ Como configurar o projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/WeslleyA/nlw_operator_iniciante.git](https://github.com/WeslleyA/nlw_operator_iniciante.git)
    ```
2.  **Configuração do Cloudinary:**
    No arquivo `index.html`, localize o objeto `config` e verifique suas credenciais:
    ```javascript
    const config = {
        cloudName: 'dwq1lx65u',
        uploadPreset: 'upload_nlw'
    }
    ```
    *Nota: Certifique-se de que o seu Upload Preset no Cloudinary esteja configurado para gerar transcrições automaticamente.*

3.  **Execução:**
    Basta abrir o arquivo `index.html` em qualquer navegador moderno.

## 📝 Como usar

1.  Clique no botão **"Upload files"**.
2.  Selecione um arquivo de vídeo ou áudio.
3.  Aguarde o processamento. O sistema tentará buscar a transcrição a cada 2 segundos.
4.  O resultado aparecerá na tela assim que o Cloudinary finalizar a análise.

---
Desenvolvido por **WeslleyA** durante o NLW da Rocketseat. 🚀


