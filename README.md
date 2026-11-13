<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1400&color=58A6FF&center=true&vCenter=true&width=680&lines=Automa%C3%A7%C3%A3o+com+Python+no+setor+jur%C3%ADdico;Rob%C3%B4s+em+produ%C3%A7%C3%A3o%2C+n%C3%A3o+em+slide;LGPD+por+padr%C3%A3o+%C2%B7+rastreabilidade+%C2%B7+revis%C3%A3o+humana" alt="Automação com Python no setor jurídico" />

# João Schwarzbach

**Software Engineer · Automação & Legaltech** · Porto Alegre, RS

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jo%C3%A3o-schwarzbach-060667290/)
[![E-mail](https://img.shields.io/badge/E--mail-joaolbschwarzbach%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:joaolbschwarzbach@gmail.com)
![Status](https://img.shields.io/badge/robôs_em_produção-sim-2EA043?style=flat-square)

</div>

```console
joao@portoalegre:~$ whoami
Software Engineer focado em automação com Python no setor jurídico.
Construo e mantenho robôs em produção que leem publicações e e-mails,
cadastram processos e conversam com iiLex, AnyTask, SharePoint e
Microsoft Graph — com LGPD, trilha de auditoria e revisão humana como
parte da definição de pronto.

joao@portoalegre:~$ git log --oneline carreira
HEAD     05/2026 → hoje    Desenvolvedor de Automação Jr · Ramos Advogados
a3f9c21  2023 → 2025       Analista de Sistemas e Operações · Daisy Vargas Ferragens
7be04d8  2021 → 2023       Jovem Aprendiz · Caixa Econômica Federal
```

## `$ stack --list`

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6-41CD52?style=for-the-badge&logo=qt&logoColor=white)
<br/>
![Microsoft Graph](https://img.shields.io/badge/Microsoft_Graph-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![SharePoint](https://img.shields.io/badge/SharePoint-0078D4?style=for-the-badge&logo=microsoftsharepoint&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=claude&logoColor=white)

</div>

## `$ cat arquitetura.md`

Como os robôs conversam no dia a dia de um escritório de advocacia:

```mermaid
flowchart LR
    A["E-mails, publicações e lotes de planilha"] --> B["ARGOS: triagem, dedup e roteamento"]
    B --> C["AnyTask BPM: cadastro automatizado"]
    B --> D["Cadastrador próprio: leitura do eproc"]
    B --> E[("SharePoint e Excel Online via Microsoft Graph")]
    C --> F[("iiLex: base de processos")]
    D --> F
    F --> G["ORÁCULO: saneamento dos campos"]
    G --> F
    F --> H["CRONOS: captura de prazos"]
    I["Bifrost"] --- F
    I --- J["Módulo jurídico do cliente"]
```

## `$ ls projetos/`

<table>
<tr>
<td width="50%" valign="top">

### ARGOS
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Suíte de 6 módulos que cruza e-mail, publicações, iiLex e SharePoint. Sincronização horária com Excel Online via **Microsoft Graph (OAuth 2.0)**, deduplicação entre fontes e trilha de auditoria de cada processo que entra.

`Python` `Microsoft Graph` `SharePoint` `Task Scheduler`

</td>
<td width="50%" valign="top">

### ORÁCULO
![](https://img.shields.io/badge/em_implantação-D29922?style=flat-square)

Sistema web interno que **saneia automaticamente os campos** de uma base de processos, 100% automático, publicado na intranet. Nasceu como app PySide6 (~3.600 linhas) com gráficos Power BI e relatórios HTML.

`Python` `PySide6` `Power BI` `pandas` `HTML/CSS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Bifrost
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Pipeline que integra iiLex, AnyTask e o módulo jurídico de um cliente: anti-duplicação, roteamento por regra e conciliação de abas de auditoria — fluxos que antes eram manuais.

`Python` `APIs REST` `openpyxl`

</td>
<td width="50%" valign="top">

### AnyTask BPM
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Robô que cadastra processos na base do iiLex: regras de leitura, montagem de lote e confirmação de cada cadastro.

`Python` `Selenium` `RPA`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### CRONOS
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Captura de prazos de publicações judiciais, auditado para corrigir durações, datas de julgamento e papel das partes. **Prazo é código crítico.**

`Python` `regex` `SQLite`

</td>
<td width="50%" valign="top">

### Classificador de publicações
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Motor com **~60 categorias** para publicações judiciais. Quando falta dado, não chuta: manda para revisão humana.

`Python` `pandas` `regex`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### BuscaJus
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Lê processos e decodifica a numeração CNJ em **92 combinações de tribunais**, com consulta O(1) em JSON.

`Python` `Selenium` `JSON`

</td>
<td width="50%" valign="top">

### ÍRIS
![](https://img.shields.io/badge/produto_próprio_·_em_desenvolvimento-8957E5?style=flat-square)

Ferramenta legaltech de código fechado: reconciliação de publicações do DJEN por OAB, **sem guardar dados do usuário**.

`Python` `FastAPI`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Infraestrutura de automação
![](https://img.shields.io/badge/em_produção-2EA043?style=flat-square)

Host Hyper-V com 4 VMs dedicadas aos robôs e uma VM com GPU para **IA local**, sem enviar dados de clientes a terceiros.

`Hyper-V` `Windows` `Entra ID`

</td>
<td width="50%" valign="top">

### Sistema NFE · Daisy Vargas Ferragens
![](https://img.shields.io/badge/entregue-57606A?style=flat-square)

Gestão fiscal desktop para uma ferragem que atende dezenas de hospitais: importa XMLs da SEFAZ, casa Ordem de Compra por padrão de cada cliente, controla estoque e entrega dashboard executivo e inteligência fiscal (NCM, CFOP, custo médio).

`Python` `PySide6` `SQLite` `lxml`

</td>
</tr>
</table>

<sub>E mais: Vigia CEJUSC (monitoramento automatizado) e o gerador de assinaturas de e-mail da intranet.</sub>

## `$ ./metricas --resumo`

| | |
|---|---|
| **12.780** bloqueios por dia investigados num rate limit | 73% vinham de uma automação de terceiros |
| **18** gargalos de produção auditados | foco em LGPD e revisão humana |
| **~60** categorias no classificador de publicações | com fila de revisão quando falta dado |
| **92** combinações de tribunais na numeração CNJ | consulta O(1) |
| **10 mil+** NF-e processadas no Sistema NFE | 22 mil+ itens, 90+ CNPJs |

## `$ cat principios.txt`

> **LGPD por padrão** — coleta mínima, dado sensível fora de log e anonimização antes de qualquer envio a terceiros.
>
> **Rastreabilidade** — toda ação relevante registra quem, quando e com base em qual fonte.
>
> **Prazo é código crítico** — regra jurídica com teste, base legal documentada e memória de cálculo auditável.

<div align="center">
<sub>joao@portoalegre:~/github · feito com Python, café e revisão humana</sub>
</div>
