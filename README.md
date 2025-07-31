# Como configurar/instalar/usar o `Wickr` no `Linux Ubuntu`

## Resumo

Neste documento estao contidos os principais comandos e configuracoes para configurar/instalar/usar o `Wickr` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings for configuring/installing/using `Wickr` on `Linux Ubuntu`._


```python
## 2. Configurar/Instalar/usar o `Git` [1]
```

## 1. Instalar o `pdftotext` no `Linux Ubuntu`

Para instalar o `pdftotext`, siga os passos abaixo:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando:
    ```bash
    sudo apt clean
    ```

    2.2 Remover pacotes `.deb` antigos ou duplicados do `cache` local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando:
    ```bash
    sudo apt autoclean
    ```

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando:
    ```bash
    sudo apt autoremove -y
    ```

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt update
    ```

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes:
    ```bash
    sudo apt --fix-broken install
    ```

    2.6 Limpar o `cache` do gerenciador de pacotes `apt` novamente:
    ```bash
    sudo apt clean
    ```

    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt list --upgradable
    ```

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt full-upgrade -y
    ```

3. Instale o `pdftotext` (pacote `poppler-utils`) e verifique a instalação:
    ```bash
    sudo apt update
    sudo apt install poppler-utils
    pdftotext -v
    ```


2. Instale o `Wickr` utilizando o Snap Store:
   ```bash
   sudo snap install wickrme
   ```
3. Execute o `Wickr` via interface grafica ou pelo terminal:
   ```bash
   wickrme
   ```
   Para executar com privilegios administrativos:
   ```bash
   sudo wickrme
   ```

### Dicas adicionais

O `Wickr` permite comunicacao segura e criptografada. Explore as configuracoes disponiveis e ajuste-as conforme suas necessidades de privacidade.

## Referencias

[1] OPENAI. ***Instalar Wickr no Ubuntu***. Disponível em: <https://chat.openai.com/share/wickr-install>. Acessado em: 31/07/2025.
