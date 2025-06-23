# 📈 Método Simplex com Interface Gráfica

Projeto desenvolvido para resolver problemas de **Programação Linear** utilizando o **Método Simplex**. A interface gráfica é construída com **Tkinter**, e a resolução do problema é feita com a biblioteca **SciPy**, tornando o processo rápido e confiável.

---

## ✅ Funcionalidades

- Interface gráfica moderna e intuitiva com **Tkinter + ThemedStyle**.
- Aceita até 4 variáveis e 5 restrições.
- Suporte completo a restrições `≤`, `≥` e `=`.
- Implementação do método Simplex via `scipy.optimize.linprog`.
- Cálculo automático de:
  - 🟢 Solução ótima.
  - 💰 Valor ótimo da função objetivo.
  - ⚖️ Preços-sombra (valores dos multiplicadores de Lagrange).

---

## 🚀 Como Executar

### 1. Instale os Requisitos

Recomenda-se criar um ambiente virtual:

```bash
python -m venv venv
venv\Scripts\activate  # No Windows
```

Instale as dependências:

```bash
pip install numpy scipy ttkthemes
```

> **Observação:** `tkinter` já vem incluso com o Python padrão (não instale via pip).

---

## 🧠 Como Usar

1. Execute o script principal:

```bash
python simplex2.py
```

2. Na interface aberta:

- Preencha os **coeficientes da função objetivo**.
- Preencha os coeficientes de até **5 restrições**, selecionando o tipo (`≤`, `≥`, `=`).
- Informe o **lado direito** de cada restrição.
- Escolha entre **Minimizar** ou **Maximizar**.
- Clique em **Resolver**.

3. O resultado será exibido logo abaixo com:

- 🟢 Solução ótima das variáveis.
- 💰 Valor ótimo da função objetivo.
- ⚖️ Preços-sombra de cada restrição.

---

## 💡 Exemplo Rápido

### Problema:

Maximizar `2x + 4y`  
Sujeito a:

- `x + 2y = 8`  
- `3x + y ≤ 12`

### Resultado esperado:

```plaintext
Solução ótima: [0.00, 4.00]
Valor ótimo: R$ 16.00
Preços-sombra (R$): [4.00, 0.00]
```

---
<!-- 
## 🧩 Estrutura do Código

- `simplex2.py`  
  Script principal com interface gráfica e integração do solver `scipy.optimize.linprog`.

### Principais Componentes

| Função | Descrição |
|--------|-----------|
| `simplex_method` | Resolve o problema com o método Simplex (SciPy). |
| `shadow_prices` | Calcula os preços-sombra com base no dual. |
| `SimplexApp` | Classe que define toda a interface e comportamento. |
| `solve` | Coleta dados da UI, chama os métodos e exibe o resultado. | -->


Este projeto foi desenvolvido como parte da disciplina **M210 - Otimização I**
<!-- 
📌 **Possíveis melhorias futuras**:

- Exibir os passos do tableau.
- Destacar variáveis básicas e não básicas.
- Exportar relatório em `.txt` ou `.pdf`.
- Suporte a mais variáveis e restrições. -->

---
