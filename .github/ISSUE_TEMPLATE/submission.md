---
name: Submissão (PT-BR)
about: Abrir uma submissão para a Rinha de Backend 2026. A engine executa os testes automaticamente.
title: "[SUBMISSÃO] "
labels: ["submissao"]
assignees: []
---

> Esse template é para **submissões**. Para reportar bug, dúvida ou sugestão, volte e escolha **Open a blank issue**.

## Checagem obrigatória

Antes de abrir a issue, confirme:

**Recursos e rede**
- [ ] Minha submissão respeita o limite de **1 unidade de CPU** e **350MB de memória**, somando todos os serviços declarados no `docker-compose.yml`.
- [ ] Meu backend escuta corretamente na **porta 9999**.
- [ ] As imagens utilizadas são compatíveis com **linux/amd64**.
- [ ] O modo de rede configurado está como **bridge** (o modo `host` não é permitido).
- [ ] Nenhum serviço está em modo **privileged**.

**Topologia**
- [ ] Tenho **pelo menos um load balancer** e **duas instâncias de API**.
- [ ] Meu load-balancer passou na lei Gabriel-2025: não tem lógica de aplicação nem responde pelas APIs (sem `~smart~ load balancing`).

**Repositório e submissão**
- [ ] Meu repositório é **público**.
- [ ] O repositório tem a branch `main` com o código-fonte e a branch `submission` com os arquivos de execução.
- [ ] A branch `submission` tem o `docker-compose.yml` na **raiz**.
- [ ] A branch `submission` tem um `info.json` preenchido.
- [ ] Abri (ou já tenho aprovado) um PR adicionando meu participante em `./participants/<meu-usuario-github>.json`.

## Execução do teste

A engine da Rinha varre issues cuja descrição contém `rinha/test` e executa os testes automaticamente. **Não remova a linha abaixo.** Se você tem mais de uma submissão, informe o `id` — por exemplo, `rinha/test ana-experimental`.

```
rinha/test
```

---

Seja feliz! 🚀
