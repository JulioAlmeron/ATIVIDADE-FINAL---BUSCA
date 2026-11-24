# 8-Puzzle — Busca em Espaço de Estados

Projeto de resolução do quebra-cabeça 8-Puzzle usando três algoritmos de busca: Busca em Largura (BFS), Busca em Profundidade (DFS) e A*.

## Implementações

- `puzzle/state.py`: geração de estados vizinhos, reconstrução do caminho e sequência de ações.
- `algorithms/bfs.py`: busca em largura, que encontra uma solução com o menor número de movimentos.
- `algorithms/dfs.py`: busca em profundidade com limite configurável (padrão: 50 movimentos).
- `algorithms/a_star.py`: busca A* com a heurística da distância Manhattan.

## Requisitos

- Python 3.10 ou superior.

## Como executar

No terminal, entre na pasta do projeto e execute:

```bash
python main.py
```

O programa apresenta a sequência de movimentos, o custo, a profundidade, a quantidade de nós expandidos e gerados e o tamanho máximo da fronteira para cada algoritmo.

## Como executar os testes

Se o projeto tiver testes na pasta `tests`, instale o pytest e execute:

```bash
python -m pip install pytest
python -m pytest
```

## Observações

- O espaço vazio é representado pelo número `0`.
- As ações são informadas em português: `CIMA`, `BAIXO`, `ESQUERDA` e `DIREITA`.
- A BFS e a A* retornam soluções de custo mínimo para este problema. A DFS respeita o limite de profundidade, mas não garante a solução mais curta.
