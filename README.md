# Cifra de Vigenère: Implementação e Criptoanálise Estatística 

Este repositório contém o **Trabalho 1** da disciplina de **Segurança Computacional (CIC0201)** do Departamento de Ciência da Computação da **Universidade de Brasília (UnB)**, sob orientação da **Profa. Priscila Solis**.

O projeto consiste no desenvolvimento de uma ferramenta em Python capaz de realizar operações de cifragem/decifragem polialfabética e um motor de ataque estatístico para recuperação automatizada de chaves.

## Funcionalidades

O sistema está dividido em dois módulos principais:

1.  **Cifrador e Decifrador:**
    *   Cifragem e decifragem de mensagens utilizando a Cifra de Vigenère.
    *   Tratamento de caracteres não alfabéticos (preservação de símbolos e espaços).
    *   Validação e normalização de chaves.

2.  **Ataque de Recuperação de Senha:**
    *   **Estimativa de Tamanho:** Utiliza o **Índice de Coincidência (IC)** para detectar a periodicidade da chave.
    *   **Análise de Frequência:** Aplica o teste de **Qui-Quadrado ($\chi^2$)** para identificar cada caractere da senha.
    *   **Suporte a Idiomas:** Tabelas de frequência integradas para **Português (PT)** e **Inglês (EN)**.

## Fundamentação Técnica

O algoritmo de criptoanálise transforma o problema polialfabético em vários problemas de substituição monoalfabética. Uma vez isoladas as colunas do criptograma, o sistema busca o deslocamento que minimize o valor de $\chi^2$, indicando a maior aderência estatística ao idioma original.

## Tecnologias Utilizadas

*   **Linguagem:** [Python 3.x](https://www.python.org/)
*   **IDE Recomendada:** [Thonny](https://thonny.org/) ou VS Code.
*   **Bibliotecas:** Apenas bibliotecas padrão (conforme restrição do roteiro).

