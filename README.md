professos: Ramon Gomes Duraes de Oliveira

# Developer Environment: Version Control & CI Good Practices

## Commandos git
working directory --> git ad
staging area --> git commit
repository

### log
```
$log --all --format=online
```

### alteracao entre versoes 
```
$ git checkout [specific_commit]
```

### cria o ambiente com as dependencias
```
$ conda env create -n devops-experiments...
```

### versao principal do codigo, default
```
$ git checkout main
```

### visualiza todas as versoes do branch ativa
```
$ git branch
```

### criar uma branch nova
```
$ git checkout -b novabranch
```
### Adicionar modificacoes inclusao e delecao (todos)
```
$ git add .
```
### ponto para aprovar as alteracoes
```
$ git commit -m "teste"
```
### mostra o status que esta na branch local
```
$ git status
```
### ignorar
adicionar no .gitignore

### resistir de algum arquivo no add . [stating area] --> [working area]
```
$ git restore --stage [nome do arquivo]
```
### exibir os logs dos commits
```
$ git log --online
```

## Visualiza tudo o que foi alterado
```
$ git diff
```

## volta do [repository] para o [staging area]
```
$ git reset
```

## Teste unitario
Garantir que a unidade do codigo esta funcionando de acordo que se espera
### Biblioteca de teste no python
pytest==7.1.*

### alterar ambiente virtual, usando o anaconda para adicionar a bibliote
```
$ conda env update -n develops-experiments-env -f env.yml
```
### Comando que executa o teste virtual
```
$ pytest
```

## Boas prática 
1. Um repositório por projeto ou solução
2. Ambiente isolado e replicáveis
3. Commits frequentes
4. Teste antes de entregar

# Collaborative development: Version Control & CI Good Practices
Ambiente colaborativo

## origem do git na nuvem
```
$ git remote
```
## Enviar o codigo da maquina para o github
-u: primeira vez que está enviando a branch para o servidor central 
```
$ git push -u origin [nome da branch]
```

## Choose a workflow: Integração contínua (CI)
Garantir que o codigo seja funcional
**AUTOMATIZAR AS ETAPAS**

biblioteca: githubactions

Sequencias de codigos que serao executadas automaticamente



