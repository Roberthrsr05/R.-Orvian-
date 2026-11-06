R. ORVIAN

Documento 09 — Documentação Técnica CSS

Versão: 1.0
Status: CSS inicial documentado
Arquivo analisado: css/style.css
Tecnologia: CSS3

⸻

1. Objetivo

Este documento apresenta a estrutura da folha de estilos do site institucional da R. Orvian.

Seu objetivo é registrar os padrões visuais, técnicas de estilização, organização dos componentes e estratégias de responsividade utilizadas no projeto.

2. Configuração global

O CSS inicia com um reset global aplicado a todos os elementos.

Propriedades utilizadas:

* margin: 0.
* padding: 0.
* box-sizing: border-box.

Essa configuração reduz diferenças de espaçamento entre elementos e facilita o controle das dimensões.

3. Estilização do documento

O elemento body define os padrões gerais da interface.

Configurações:

* Fonte: Arial, Helvetica, sans-serif.
* Fundo: #101827.
* Texto: #F3F5F8.
* Altura de linha: 1.6.

Os links recebem configurações globais para remover o sublinhado e herdar a cor do elemento pai.

4. Sistema de cores

A identidade visual utiliza uma paleta baseada em tons escuros e azuis.

Cor	Código	Aplicação
Azul elétrico	#3988F5	Destaques e interações
Fundo principal	#101827	Fundo da página
Fundo secundário	#1C2B40	Menus e cards
Branco	#FFFFFF	Títulos e destaques
Texto claro	#DCE6F2	Textos secundários
Cinza azulado	#8FA3BF	Rodapé
Bordas	#344761	Separação de componentes

5. Cabeçalho e navegação

O componente .topo utiliza Flexbox.

Propriedades principais:

* display: flex.
* justify-content: space-between.
* align-items: center.
* flex-wrap: wrap.
* max-width: 1200px.

A navegação principal também utiliza Flexbox para organizar os links horizontalmente.

Os links possuem transição de cor e destaque azul no estado hover.

6. Menu adicional

O menu adicional utiliza a classe .menu-extra.

Sua apresentação é controlada por CSS, enquanto sua abertura e fechamento são realizados pelo elemento HTML details.

Recursos implementados:

* Posicionamento relativo do componente.
* Posicionamento absoluto das opções.
* Fundo escuro.
* Bordas arredondadas.
* Destaque visual no estado aberto.
* Efeito de hover.
* Indicador de foco com focus-visible.
* Animação de entrada utilizando @starting-style.

O menu utiliza um tamanho mínimo de 44 × 44 pixels para a área interativa do botão.

7. Conteúdo principal

O elemento main utiliza largura de 90%, limitada a 1200 pixels, com centralização automática.

A seção .hero utiliza:

* Alinhamento centralizado.
* Largura máxima de 700 pixels.
* Espaçamento inferior.
* Tipografia adaptável.

O título principal utiliza a função clamp() para ajustar seu tamanho conforme a largura da tela.

8. Botão institucional

O componente .botao apresenta:

* Fundo azul.
* Texto branco.
* Bordas arredondadas.
* Cursor de interação.
* Transição de cor.
* Efeito de elevação no hover.
* Indicador de foco por teclado.

O botão possui destaque visual consistente com a identidade da marca.

9. Organização dos cards

A classe .areas utiliza CSS Grid.

Configuração principal:

grid-template-columns: repeat(auto-fit, minmax(min(250px, 100%), 1fr));

Essa configuração permite que os cards se reorganizem conforme o espaço disponível.

Os elementos article apresentam:

* Fundo secundário.
* Bordas.
* Cantos arredondados.
* Espaçamento interno.
* Transição visual.
* Elevação no hover.

10. Rodapé

O elemento footer utiliza:

* Texto centralizado.
* Espaçamento interno.
* Borda superior.
* Cor secundária.
* Tamanho de fonte reduzido.
* Espaçamento entre caracteres.

11. Responsividade

O projeto utiliza media queries para adaptar a interface.

11.1. Tablet — até 900 pixels

Ajusta o espaçamento vertical do conteúdo principal e da seção Hero.

11.2. Celular — até 600 pixels

Implementa:

* Cabeçalho em coluna.
* Redução do tamanho do título institucional.
* Ajuste da navegação.
* Redução dos espaçamentos.
* Botão com largura total.
* Redução do espaçamento interno dos cards.

12. Dispositivos sem mouse

O projeto utiliza:

@media (hover: none)

Essa regra remove os efeitos de transformação dos cards e do botão em dispositivos sem capacidade de hover.

Isso evita que os efeitos de elevação sejam aplicados de maneira inadequada em interfaces baseadas em toque.

13. Acessibilidade

O CSS apresenta recursos importantes:

* Indicadores de foco com focus-visible.
* Área interativa mínima de 44 × 44 pixels no menu adicional.
* Contraste visual entre fundo e conteúdo.
* Estados visuais para elementos interativos.

Como melhoria futura, recomenda-se implementar suporte à preferência prefers-reduced-motion para usuários que preferem animações reduzidas.

14. Tecnologias e recursos utilizados

* CSS3.
* Flexbox.
* CSS Grid.
* Media Queries.
* Transitions.
* Transform.
* Clamp.
* Min.
* Minmax.
* Focus-visible.
* Starting-style.

15. Considerações finais

A folha de estilos estabelece a identidade visual inicial da R. Orvian, utilizando uma estrutura organizada e recursos modernos de CSS.

A implementação prioriza consistência visual, adaptação a diferentes dispositivos e facilidade de manutenção.

Futuras alterações deverão preservar a identidade visual e acompanhar a evolução do HTML e das funcionalidades do projeto.

⸻

R. ORVIAN
Tecnologia para transformar possibilidades em soluções.

Documento interno — Documentação Técnica CSS.