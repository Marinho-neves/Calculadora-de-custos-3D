# Calculadora de preço 3D

Calculadora web para precificar peças impressas em 3D. Roda direto no navegador, sem instalação e sem dependências.

## O que ela calcula

- Filamento (com margem para falhas e desperdício)
- Energia elétrica
- Desgaste da máquina
- Seu tempo de trabalho
- Embalagem e extras
- Preço final com margem de lucro e taxa de plataforma

Também é possível informar o nome do serviço (peça) e do cliente, imprimir um orçamento limpo para o cliente (sem mostrar custos nem margem) e limpar todos os campos com um clique.

O resultado mostra o preço por peça, o lucro e o total para a quantidade informada. Os valores digitados ficam salvos no navegador (localStorage).

## Como usar

Abra o `index.html` no navegador.

## Publicar no GitHub Pages

1. Envie `index.html` e `README.md` para um repositório.
2. Vá em **Settings → Pages**.
3. Em **Source**, escolha a branch `main` e a pasta `/ (root)`.
4. Salve. O site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Fórmula

```
custo = filamento + energia + máquina + trabalho + embalagem
preço = custo / (1 - margem - taxa)
```

Onde margem e taxa são percentuais sobre o preço de venda.
