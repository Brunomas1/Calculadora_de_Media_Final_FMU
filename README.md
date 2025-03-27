# Calculadora de Média Final da Disciplina Online

Este projeto consiste em uma calculadora interativa desenvolvida para ser executada no Google Colab, utilizando Python e a biblioteca `ipywidgets`. A calculadora calcula a média final de uma disciplina online, aplicando regras específicas de avaliação, e exibe o resultado com uma formatação adaptativa para dark mode e light mode.

## Descrição

Na disciplina online, a avaliação é dividida em duas etapas:

- **Primeira Etapa (N1):**
  - São consideradas as atividades avaliativas A1, A2, A3 e A4.
  - Cada atividade vale até 10,0 pontos.
  - A média de N1 é calculada como a média aritmética das quatro atividades.

- **Segunda Etapa:**
  - Envolve a Prova N2 (A5) e, opcionalmente, a Prova Substitutiva (A6).
  - Se ambas as provas forem informadas, a maior nota é considerada para o cálculo.
  
- **Cálculo da Nota Final:**
  - A Nota Final é calculada pela média ponderada entre N1 (40%) e a nota de exame (A5 ou A6, 60%):
  
    \[
    \text{Nota Final} = (N1 \times 0.4) + (\text{Exame} \times 0.6)
    \]
  
  - A aprovação na disciplina exige Nota Final igual ou superior a 6,0.

Além disso, o projeto inclui um bloco de CSS que ajusta a aparência do resultado final automaticamente, garantindo boa visualização em qualquer tema (dark ou light).

## Funcionalidades

- **Interface Interativa:** Utiliza `ipywidgets` para entrada de dados e interatividade.
- **Validação de Notas:** Realiza validação para garantir que as notas estejam entre 0 e 10, tratando entradas vazias e inválidas.
- **Resultado Formatado:** Exibe o resultado final com HTML, incluindo a média N1, a nota utilizada da prova e a Nota Final, além de mensagens de aprovação ou reprovação.
- **Aparência Adaptativa:** Usa media queries em CSS para adaptar as cores do resultado conforme o tema do Colab (dark/light).

## Como Utilizar

1. **Abrir no Google Colab:**
   - Acesse o notebook interativo diretamente através do seguinte link:
     
     [Abrir no Google Colab](https://colab.research.google.com/drive/1ezdAGoNnM8rfr5k6IBuixBczU62lXJCM?usp=sharing)
     
   - Você também pode criar um novo notebook no [Google Colab](https://colab.research.google.com/) e copiar o código fonte da calculadora (disponível neste repositório) em uma célula.

2. **Executar a Célula:**
   - Execute a célula para carregar a interface interativa.
   - Insira as notas para as atividades A1, A2, A3 e A4.
   - Insira a nota da Prova N2 (A5) e, se aplicável, a Prova Substitutiva (A6).
   - Clique no botão **Calcular** para visualizar o resultado final.

## Requisitos

- Python 3.x
- [Google Colab](https://colab.research.google.com/)
- Biblioteca `ipywidgets`

Para instalar a biblioteca `ipywidgets` (caso esteja utilizando um ambiente local), execute:

```bash
pip install ipywidgets
