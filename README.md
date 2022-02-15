# LinuxCommands
Comandos básicos utilizados no emulador de terminal Linux.

### Atalhos do emulador de terminal
- `Tab`: realiza o autocompletar de comandos e diretórios.
- `Ctrl+a`: posiciona o cursor no início do comando.
- `Ctrl+e`: posiciona o cursor no final do comando.
- `Ctrl+l`: equivalente ao comando `clear`, limpa todo o terminal.
- `Ctrl+c`: encerra o processo em execução.
- `Ctrl+d`: equivalente ao comando `exit`, fecha o terminal.

### Comandos gerais

Navegar entre os diretórios:
```
$ cd ".../"
```

Ir para o diretório anterior:
```
$ cd ..
```

Abrir manual de algum comando:
```
$ man "COMANDO"
```

Mostrar hostname:
```
$ hostname
```

Mostrar diretório atual:
```
$ pwd
```

Criar arquivo vazio:
```
$ touch "NOME"
```

Criar pasta no diretório atual:
```
$ mkdir "NOME"
```


Listar arquivos no diretório atual:
```
$ ls
$ ls -l (permissões)
$ ls -a (ocultos)
$ ls -lh (incluir tamanho)
```

Ler arquivo de texto:
```
$ cat "ARQUIVO"
```

Mover/renomiar arquivo:
```
$ mv "ORIGEM" "DESTINO"
```

Copiar arquivo:
```
$ cp "ORIGEM" "DESTINO"
```

Remover arquivo
```
$ rm "ARQUIVO"
```

Mostrar usuário:
```
$ whoami
```

Zipagem de arquivos ou pastas 
> (zip; nome do arquivo zipado; arquivo que será zipado)
> O arquivo que será zipado não é deletado

```
$ zip zipado.zip "ARQUIVO" "pasta/*"
```
> para descompactar algum .zip, utiliza-se:
```
unzip arquivo.zip
```

Buscar arquivos
> (find; diretório que será vasculhado; flag; nome ou formato)
> é retornado o diretório em que encontra-se o arquivo procurado
 
```
find ./ -name ‘*.cpp’
```
