# Uma Fórmula Combinatória para Contagem de Elementos Lineares em Grades Retangulares: Derivação e Aplicações

## Resumo
Este artigo apresenta uma fórmula combinatória para calcular o número de elementos lineares (como palitos, juntas ou vigas) em estruturas retangulares compostas por quadrados unitários. A expressão $[(x^2 + x) + (y^2 + y)] - (y - x)^2$ é derivada a partir de princípios básicos de contagem e simplificada para $x + y + 2xy$. Aplicações em construção civil (cálculo de rejunte, vigas e barras) são discutidas com rigor matemático.

## 1. Introdução
Estruturas retangulares compostas por quadrados unitários aparecem em diversos contextos, como grades de palitos, revestimentos de azulejos e treliças. Este artigo deriva uma fórmula geral para contar o número de elementos lineares nessas estruturas, partindo de um caso específico (grade $5 \times 4$ de palitos) e generalizando para aplicações práticas. A fórmula é apresentada em sua forma original e simplificada, com demonstrações algébricas rigorosas.

## 2. Derivação a Partir de um Caso Específico: Grade $5 \times 4$
Considere uma grade retangular de quadrados unitários formada por palitos, com $x = 5$ colunas e $y = 4$ linhas. Cada quadrado é delimitado por palitos de comprimento unitário.

### 2.1 Contagem Direta dos Palitos
- **Palitos horizontais**: Existem $y + 1 = 5$ linhas horizontais, cada uma com $x = 5$ palitos.  
  Total: $5 \times 5 = 25$.
- **Palitos verticais**: Existem $x + 1 = 6$ linhas verticais, cada uma com $y = 4$ palitos.  
  Total: $6 \times 4 = 24$.
- **Total de palitos**: $25 + 24 = 49$.

### 2.2 Generalização para uma Grade $x \times y$
Para uma grade com $x$ colunas e $y$ linhas:
- Palitos horizontais: $(y + 1)x$
- Palitos verticais: $(x + 1)y$
- Total de palitos:
$$
N = x(y + 1) + y(x + 1) = 2xy + x + y \tag{1}
$$

## 3. Derivação da Fórmula Original
A fórmula proposta é:
$$
F = [(x^2 + x) + (y^2 + y)] - (y - x)^2
$$
Expandindo os termos:
$$
F = x^2 + x + y^2 + y - (y^2 - 2xy + x^2) = x^2 + x + y^2 + y - y^2 + 2xy - x^2 = x + y + 2xy
$$
Que é idêntica à Equação (1). Portanto, $F = N$.

### 3.1 Interpretação Combinatória
A forma original $F$ pode ser interpretada como:
- $x^2 + x$: Soma do número de palitos horizontais se cada quadrado fosse independente (sem compartilhamento), ajustado pelas bordas.
- $y^2 + y$: Analogamente para palitos verticais.
- A subtração de $(y - x)^2$ corrige sobrecontagens devido à diferença dimensional, garantindo a contagem precisa dos palitos compartilhados.

## 4. Generalização para Aplicações Práticas
### 4.1 Cálculo de Rejunte em Revestimentos
Para azulejos quadrados de lado $L$:
- $x$: número de azulejos na horizontal.
- $y$: número de azulejos na vertical.
- Comprimento total das juntas (rejunte):
$$
L_{\text{total}} = L \cdot (2xy + x + y)
$$
- Volume de rejunte (com largura $w$ e profundidade $p$):
$$
V = w \cdot p \cdot L \cdot (2xy + x + y)
$$
**Exemplo**: Para uma parede com $x = 10$ azulejos de $0,3$ m, $y = 8$ azulejos, $w = 0,01$ m, $p = 0,01$ m:
$$
L_{\text{total}} = 0,3 \cdot (2 \cdot 10 \cdot 8 + 10 + 8) = 0,3 \cdot 178 = 53,4 \text{ m}
$$
$$
V = 0,01 \cdot 0,01 \cdot 53,4 = 0,00534 \text{ m}^3 = 5,34 \text{ litros}
$$
Adicionando 10% para desperdício: $5,34 \times 1,1 \approx 5,87$ litros.

### 4.2 Vigas e Barras em Estruturas
Para uma treliça com $x$ vigas horizontais e $y$ verticais (comprimento unitário $L$):
- Número total de barras: $2xy + x + y$
- Comprimento total de material: 
$$
L_{\text{total}} = L \cdot (2xy + x + y)
$$
**Exemplo**: Para $x = 10$, $y = 8$, $L = 2$ m:
$$
L_{\text{total}} = 2 \cdot (2 \cdot 10 \cdot 8 + 10 + 8) = 2 \cdot 178 = 356 \text{ m}
$$

### 4.3 Adaptações para Não Unitariedade
Se os elementos não forem unitários, com dimensões $a \times b$:
- Ajuste: $x = X/a$, $y = Y/b$, onde $X$ e $Y$ são as dimensões totais da estrutura.
- O comprimento total é então:
$$
L_{\text{total}} = a \cdot b \cdot \left(2 \cdot \frac{X}{a} \cdot \frac{Y}{b} + \frac{X}{a} + \frac{Y}{b}\right) = 2XY + aY + bX
$$
(após simplificação, dependendo do contexto).

## 5. Conclusão
A fórmula $[(x^2 + x) + (y^2 + y)] - (y - x)^2$ fornece uma expressão compacta e matematicamente elegante para problemas de contagem linear em estruturas retangulares. Sua derivação a partir de princípios combinatórios e sua aplicabilidade em contextos práticos destacam sua utilidade. Generalizações para elementos não unitários são diretas, tornando-a uma ferramenta versátil para engenheiros e matemáticos.

## Referências
- Graham, R. L., Knuth, D. E., Patashnik, O. (1994). *Concrete Mathematics*. Addison-Wesley.
- Engel, A. (1998). *Problem-Solving Strategies*. Springer.
