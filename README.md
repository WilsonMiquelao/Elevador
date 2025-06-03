# Simulador de Elevador

Projeto em Python que simula o funcionamento básico de um elevador. O sistema controla a quantidade de pessoas e os andares acessíveis, respeitando limites de capacidade e altura.

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**: Linguagem principal do projeto
- **Programação Orientada a Objetos (POO)**: Uso de classe para representar o elevador
- **Interface por terminal**: Saída e entrada via `print()` e `input()` (caso seja estendido)

---

## 📋 Funcionalidades

- ✅ Subir andares (respeitando o limite máximo)
- ✅ Descer andares (não permite ir abaixo do térreo)
- ✅ Entrar pessoas (até a capacidade máxima)
- ✅ Sair pessoas (não permite sair se estiver vazio)

---

## 🧠 Estrutura da Classe

### Classe `Elevador`

#### Atributos

- `totalCapacidade`: capacidade máxima de pessoas
- `atualCapacidade`: quantidade atual de pessoas
- `totalAndar`: número máximo de andares
- `atualAndar`: andar atual do elevador

#### Métodos

- `subir()`: sobe um andar (se possível)
- `descer()`: desce um andar (se possível)
- `entrar()`: adiciona uma pessoa ao elevador
- `sair()`: remove uma pessoa do elevador

---

## 💡 Exemplo de Uso

```python
e = Elevador(5, 10)  # Elevador com capacidade para 5 pessoas e 10 andares

e.entrar()
e.subir()
e.subir()
e.sair()
e.descer()
