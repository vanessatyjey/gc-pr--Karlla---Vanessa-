# Prática de Pull Request

Projeto-base da aula 04 de Gerência de Configuração (UNIGRAN, 2026/2). São três arquivos Python
pequenos, com defeitos de propósito: cada defeito vira uma issue, um ramo, um pull request e um merge.

## Como rodar

```bash
python main.py
```

No Windows, se `python` não for reconhecido, use `py main.py`.

## Estrutura

| Arquivo | O que é |
|---|---|
| `saudacao.py` | mensagens: hello world, saudação e despedida |
| `calculadora.py` | operações: somar, subtrair e média |
| `main.py` | o programa: chama as funções e mostra o resultado |

## Regras de versionamento

- Toda mudança começa por uma **issue**, com o que acontece hoje, o que deveria acontecer e o
  critério de aceite.
- O trabalho é feito em um **ramo por issue**, nomeado `tipo/numero-descricao` (`fix/1-saudacao`).
- As mensagens de commit seguem o padrão **Conventional Commits**: `tipo: resumo`, com `Refs #N` no
  rodapé quando houver corpo.
- Nada entra no `main` sem **pull request** revisado por outra pessoa. A descrição do PR traz
  `Closes #N`, e é o merge que fecha a issue.
