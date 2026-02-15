# Solução Numérica para EDOs de Segunda Ordem usando RK4
# Numerical Solver for Second-Order Ordinary Differential Equations using RK4
---
## <img src="https://flagcdn.com/w20/br.png" width="20"/> Versão em Português

### Visão Geral

Este projeto implementa o método de Runge-Kutta de quarta ordem (RK4)
para resolver numericamente equações diferenciais ordinárias (EDOs) de segunda ordem da forma:

    y'' = f(t, y, y')

A equação é transformada em um sistema equivalente de primeira ordem,
ao qual se aplica o método RK4 para obter uma aproximação numérica da solução.

A implementação pode ser aplicada a sistemas físicos como:
- Osciladores harmônicos
- Sistemas com amortecimento
- Modelos de vibração mecânica
- Aproximações básicas de ondas acústicas

---

### Formulação Matemática

Qualquer EDO de segunda ordem:

    y'' = f(t, y, y')

pode ser reescrita como:

    y₁ = y
    y₂ = y'

Então:

    y₁' = y₂
    y₂' = f(t, y₁, y₂)

O método RK4 é aplicado a esse sistema equivalente.

O método apresenta:
- Erro local de truncamento: O(h⁵)
- Erro global: O(h⁴)

---

### Exemplo: Oscilador Harmônico Amortecido

A equação:

    y'' + C y' + K y = 0

é reescrita como:

    y'' = -C y' - K y

onde:
- K representa a rigidez do sistema
- C representa o coeficiente de amortecimento

A simulação numérica evidencia a diferença entre o comportamento amortecido e não amortecido.

---

### Como Executar

1. Clone o repositório:

    git clone <link-do-repositório>

2. Instale as dependências:

    pip install numpy matplotlib

3. Execute o arquivo:

    python rk4_para_resolução_de_edos.py

---

## <img src="https://flagcdn.com/w20/us.png" width="20"/> English Version

### Overview

This project implements the Fourth-Order Runge-Kutta (RK4) method 
to numerically solve second-order ordinary differential equations (ODEs) of the form:

    y'' = f(t, y, y')

The method transforms the second-order equation into an equivalent 
first-order system and applies the RK4 scheme to approximate the solution.

This implementation can be applied to physical systems such as:
- Harmonic oscillators
- Damped oscillations
- Mechanical vibration models
- Basic acoustic wave approximations

---

### Mathematical Formulation

Any second-order ODE:

    y'' = f(t, y, y')

can be rewritten as the system:

    y₁ = y
    y₂ = y'

Then:

    y₁' = y₂
    y₂' = f(t, y₁, y₂)

The RK4 method is applied to this system.

The method has:
- Local truncation error: O(h⁵)
- Global error: O(h⁴)

---

### Example: Damped Harmonic Oscillator

The equation:

    y'' + C y' + K y = 0

is rewritten as:

    y'' = -C y' - K y

where:
- K is the stiffness parameter
- C is the damping coefficient

The numerical simulation illustrates the difference between damped and undamped oscillatory behavior.

---

### How to Run

1. Clone the repository:

    git clone <your-repository-link>

2. Install dependencies:

    pip install numpy matplotlib

3. Run the script:

    python rk4_para_resolução_de_edos.py

---

### Project Structure

- rk4_para_resolução_de_edos.py → General RK4 solver
- example_plot.png → Simulation output
- README.md → Documentation

---

### Future Improvements

- Adaptive step-size RK methods
- Error analysis against analytical solutions
- Nonlinear system extensions
- Applications to acoustic signal modeling

--- 

###  Autor

Felipe Rodrigues Chaves  
