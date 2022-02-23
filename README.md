# **LinuxCommands**

Comandos básicos utilizados no emulador de terminal Linux.

## **Atalhos do emulador de terminal**

- `Tab`: realiza o autocompletar de comandos e diretórios.
- `Ctrl+a`: posiciona o cursor no início do comando.
- `Ctrl+e`: posiciona o cursor no final do comando.
- `Ctrl+l`: equivalente ao comando `clear`, limpa todo o terminal.
- `Ctrl+c`: encerra o processo em execução.
- `Ctrl+d`: equivalente ao comando `exit`, fecha o terminal.

## Navegação


- Navegar entre os diretórios:
    
    ```
    cd ".../"
    ```
    
- Ir para o diretório anterior:
    
    ```
    cd ..
    ```

## Mostrar informações


- Mostrar diretório atual:
    
    ```
    pwd
    ```
    
- Listar arquivos no diretório atual:
    
    ```
    ls
    ls -l (permissões)
    ls -a (ocultos)
    ls -lh (incluir tamanho)
    ```
    
- Ler arquivo de texto:
    
    ```
    cat "ARQUIVO"
    ```
    
    
    - Abrir manual de algum comando:
    
    ```
    man "COMANDO"
    ```
    
    
- Contagem de linhas, palavras e bytes de um arquivo:
    
    ```
    wc -l           # retorna a quantidade de linhas
    ```
    
    
- Mostrar usuário:
    
    ```
    whoami
    ```
    
- Mostrar hostname:
    
    ```
    hostname
    ```
    

## Criar e deletar


- Criar arquivo vazio:
    
    ```
    touch "NOME"
    ```
    
- Criar pasta no diretório atual:
    
    ```
    mkdir "NOME"
    ```
    
- Remover arquivo vazio:
    
    ```
    rm "ARQUIVO"
    ```
    
- Remover diretório vazio:
    
    ```
    rmdir "diretórios"
    ```
    
- Remover diretório com conteúdo:

    ```
    rm -r "diretórios"
    ```
    
## Manipulação de arquivos de texto

- Sobre-escrever texto
 
 ```
 echo 'Hello, world!' > "ARQUIVO.TXT"  
 echo > "ARQUIVO"           # irá limpar o arquivo
 ```
 
 - Concatenar texto

```
echo uva >> melhoresFrutas.txt
```

    
- Redirecionar conteúdo entre arquivos

```
cat "ARQUIVO-FONTE" > "ARQUIVO-DESTINO"
```

# Manipulação de dados

- Identificar quantidade de ocorrência

```
ls -l | grep '.txt'                          # retorna a quantidade de arquivos terminados .txt
grep 'banana' vendas.txt                     # retorna todas as ocorrências ‘banana’ no texto
```

## Mover, copiar e renomear


- Mover/renomear arquivo:
    
    ```
    mv "ORIGEM" "DESTINO"
    ```
    
- Copiar arquivo:
    
    ```
    cp "ORIGEM" "DESTINO"
    ```
    

## Zipagem


- Zipar arquivo
    
    ```
    zip zipado.zip "ARQUIVO" "pasta/*"
    ```
    

> (zip; nome do arquivo zipado; arquivo que será zipado) O arquivo que será zipado não é deletado
> 
- Descompactar algum .zip:
    
    ```
    unzip arquivo.zip
    ```
    
- Buscar arquivos

> (find; diretório que será vasculhado; flag; nome ou formato) é retornado o diretório em que encontra-se o arquivo procurado
> 

```
find ./ -name ‘*.cpp’
```
