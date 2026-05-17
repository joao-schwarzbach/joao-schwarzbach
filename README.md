<div align="center">

# João Schwarzbach

**Desenvolvedor Python · Sistemas fiscais e ferramentas internas**

Construo desktop apps em PySide6 que tiram planilha e processo manual do meio do caminho — gestão de NFe, validação de bases de processos, BI executivo e automação de rotina.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6-41CD52?style=for-the-badge&logo=qt&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

</div>

---

## Projetos em destaque

### Sistema NFE — Daisy Vargas Ferragens

Sistema desktop completo de gestão fiscal e movimentação de notas para uma ferragem que atende dezenas de hospitais. Importa XMLs da SEFAZ direto da pasta do Gestão Click, descompacta ZIPs, extrai itens, casa Ordem de Compra por padrão de cada cliente, controla saída de estoque e entrega dashboard executivo + ranking de clientes + inteligência fiscal (NCM, CFOP, custo médio ponderado).

- **Stack:** Python · PySide6 · SQLite · pandas · lxml · PyInstaller
- **Volume real:** 10k+ NFes processadas, 22k+ itens, 90+ CNPJs distintos
- **Diferenciais:** parsing de OC com mapa de padrões por hospital (UBEA, AESC, GHC, HCPA, Moinhos, Santa Casa, UNIMED…), backups automáticos do banco, atalhos de teclado (F5, Ctrl+F), exportação Excel
- **UI:** tema escuro próprio ("Oráculo") com header LED pulsante, cards, tabelas Qt customizadas

### Oráculo — Ramos Advogados

Ferramenta de saneamento e validação da base de processos de um escritório de advocacia. Lê a base operacional, aplica regras de consistência (campos faltantes, divergências entre planilhas, status incompatíveis), gera planilha de erros classificados e um relatório HTML pronto pra mandar pra controladoria.

- **Stack:** Python · PySide6 · pandas · openpyxl
- **Saída:** planilha de erros (.xlsx) + relatório HTML formatado
- **UX:** interface single-screen, dark mode, log em tempo real do processamento
- **Identidade visual:** paleta azul-noite #0F1923 com destaque vermelho #C00000 — virou a referência de design que reuso nos outros projetos

---

## O que eu uso

```
Linguagens   Python, SQL
GUI          PySide6 / Qt
Dados        pandas, openpyxl, lxml, SQLite
Build        PyInstaller (executáveis Windows standalone)
Domínio      NFe/SEFAZ, regras fiscais, automação de planilhão
```

---

## Contato

- E-mail: **joaolbschwarzbach@gmail.com**
- WhatsApp: **(51) 99537-0669**

<div align="center">

<sub>Sistemas reais, rodando em produção, resolvendo problema de quem usa planilha.</sub>

</div>
