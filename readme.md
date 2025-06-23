# 📈 Método Simplex com Interface Gráfica

Projeto desenvolvido para resolver problemas de **Programação Linear** utilizando o **Método Simplex**. A interface gráfica é construída com **Tkinter**, permitindo fácil interação com o usuário.

---

## ✅ Funcionalidades

- Interface gráfica intuitiva (Tkinter).
- Aceita problemas com 2 ou mais variáveis e restrições.
<!-- - Suporte completo a restrições `<=`, `>=` e `=`. -->
- Implementação completa do Método Simplex.
- Exibe:
  - 🟢 Solução ótima.
  - 💰 Valor ótimo da função objetivo.
  <!-- - ⚖️ Preços sombra (fase futura - opcional). -->

---

## 🚀 Como Executar

### 1. Instale os Requisitos

Crie um ambiente virtual (opcional, mas recomendado):

```bash
python -m venv venv
venv\Scripts\activate  # Windows
```

Instale as dependências:

```bash
pip install numpy
```

> **Nota:** Não é necessário instalar `tkinter` via `pip`. Ele já vem incluso no Python padrão (distribuição oficial).

---

## 🧠 Como Usar

1. Execute o script `simplex.py`:
   ```bash
   python simplex.py
   ```

2. Na interface:
   - Informe o número de variáveis e restrições.
   - Clique em **"Gerar Campos"**.
   - Preencha:
     - Coeficientes da função objetivo.
     - Coeficientes de cada restrição.
     <!-- - Operador (`<=`, `>=`, `=`). -->
     - Termo constante (lado direito).
   - Clique em **"Calcular"**.

3. O resultado será exibido em uma janela com:
   - Solução ótima.
   - Valor ótimo.

---

<!-- ## 💡 Exemplo de Entrada

- Função objetivo: `Max Z = 3x₁ + 2x₂`
- Restrições:
  - `x₁ + x₂ ≤ 4`
  - `2x₁ + x₂ ≤ 5`

### Resultado Esperado:

```plaintext
Solução ótima: [0.0, 0.0]
Valor ótimo: 0.0000
``` -->
<!-- 
> Para outro exemplo com resultado positivo:
>
> - FO: `Max Z = 3x₁ + 5x₂`
> - Restrições:
>   - `x₁ ≤ 4`
>   - `2x₂ ≤ 12`
>
> **Resultado:** `x₁ = 4`, `x₂ = 6`, `Z = 3*4 + 5*6 = 38` -->

---

## 🧩 Estrutura do Código

- `simplex.py`  
  Implementação do método Simplex com duas fases + interface gráfica.

### Principais Componentes

| Função | Descrição |
|--------|-----------|
| `simplex` | Resolve o problema usando o método Simplex com variáveis artificiais. |
| `executar` | Coleta dados da interface e chama o solver. |
| `gerar_campos` | Gera dinamicamente os campos de entrada conforme o número de variáveis/restrições. |
| `root.mainloop()` | Inicializa a interface Tkinter. |

---

<!-- ## ⚠️ Possíveis Erros

- **Erro de shape `inhomogeneous shape`**: ocorre quando as restrições têm comprimentos diferentes. Isso foi corrigido com tratamento uniforme das colunas extras.
- **Problemas sem solução viável**: o programa detecta e alerta o usuário.

--- -->

## 👨‍🎓 Público-Alvo

- Estudantes de Engenharia, Matemática Aplicada, Administração e áreas correlatas.
- Professores que queiram demonstrar o algoritmo Simplex visualmente.
- Qualquer pessoa interessada em otimização linear.

---

## 🏁 Considerações Finais

Este projeto foi desenvolvido como parte da disciplina **M210 - Otimização I**, com foco em:

- Clareza de implementação.
- Interface acessível.
- Rigor na resolução de problemas com diferentes tipos de restrições.
<!-- 
📌 **Futuras melhorias possíveis**:
- Exibir passos intermediários do tableau.
- Mostrar as variáveis básicas e não básicas ao final.
- Exportar relatório em `.txt` ou `.pdf`. -->

---