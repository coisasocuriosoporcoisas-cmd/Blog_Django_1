# Requisitos do projeto

Este projeto é um blog Django que usa SQLite, tags para posts, formatação
Markdown e os recursos de administração e testes do Django.

## Python

Instale uma versão do Python compatível com a versão do Django fixada no
`requirements.txt`.

## Pacotes Python

As versões abaixo são as registradas em `requirements.txt`:

| Pacote | Versão | Uso |
| --- | --- | --- |
| Django | 6.1.1 | Framework web, ORM, templates, administração e testes |
| django-taggit | 5.0.1 | Tags associadas aos posts |
| Markdown | 3.6 | Conversão de conteúdo Markdown |
| asgiref | 3.12.1 | Dependência do Django para suporte a ASGI e código assíncrono |
| sqlparse | 0.6.0 | Dependência do Django para formatação e análise de SQL |
| tzdata | 2026.4 | Dados de fuso horário, necessários em ambientes sem a base do sistema |

`asgiref`, `sqlparse` e `tzdata` acompanham a lista para manter as versões
instaladas reproduzíveis. O SQLite usado pelo projeto já faz parte da biblioteca
padrão do Python e não precisa de pacote Python separado.

## Instalação

Na pasta raiz do repositório, crie e ative um ambiente virtual no PowerShell e
instale as dependências:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```
