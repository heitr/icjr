---
header-includes: \usepackage{mhchem}
title: |
       | ![](logo.png){ width=80px }
       | **Centro Federal de Educação Tecnológica de Minas Gerais**
       |
       | Grupo de Química para Simulações *In Silico*
subtitle: Manual de uso dos *scripts*
author: Heitor Leite
---

# Introdução

Scripts são arquivos contendo sequências de comandos a serem executados pelo sistema a fim de realizar alguma tarefa.

## Instalação

O script de instalação baixa e instala automaticamente a última versão disponível dos scripts. Ele pode ser acessado na página [git.io/scripts_ic](https://git.io/scripts_ic). Para executá-lo basta usar o seguinte comando:

```sh
source <(curl -sL git.io/scripts_ic)
```

# Descrição

## substitui
Substitui um elemento e sua multiplicidade em todos arquivos `.inp` de um diretório e seus subdiretórios.

## verifica
Verifica se o cálculo de um arquivo `.out` foi bem sucedido e faz a análise vibracional.

## gera_script_srm
Gera um script `.srm` que pode ser submetido ao comando `sbatch` para todo arquivo `.inp` de um diretório e seus subdiretórios.

## lista_jobs

Lista os *jobs* do usuário atual no *slurm* mostrando o nome completo de cada *job*.

## gera_csv
Verifica o resultado de todos os arquivos `.out` de um diretório e seus subdiretórios e gera uma tabela `.csv` com os dados relevantes (energia eletrônica, energia livre de gibbs e entalpia total).
