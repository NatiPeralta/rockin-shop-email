Processo de desenvolvimento do teste Rockin' Shop:

Por ser a minha primeira experiência desenvolvendo um e-mail marketing com HTML e CSS, iniciei o processo com pesquisas sobre as melhores práticas específicas para esse tipo de implementação, entendendo que o desenvolvimento para e-mail possui características diferentes do desenvolvimento web tradicional.

Durante esse estudo, identifiquei alguns pontos essenciais:

- Utilização de estruturas <table> para construção do layout, garantindo maior compatibilidade entre diferentes clientes de e-mail;

- Uso de CSS inline, prática recomendada para melhor renderização em provedores como Gmail e Outlook;

- Largura padrão entre 600px e 800px, sendo 600px o valor mais seguro e amplamente utilizado;

- Responsividade adaptada com largura fluida (100%), considerando as limitações de suporte a media queries em alguns clientes;

- Importância de manter um bom equilíbrio entre texto e imagens, evitando problemas com filtros de spam;

- Necessidade de testes em ferramentas como Litmus ou Email on Acid para validação da renderização.

Utilizei o layout base como referência visual para desenvolvimento. Ao manter ele aberto no Canva, obtive facilidade com a extração de cores, proporções e estilos tipográficos.

Um dos primeiros desafios foi encontrar imagens com qualidade adequada para uso no e-mail. Após alguns testes, utilizei o Canva para ajustar e exportar os assets, buscando preservar a melhor resolução possível dentro das limitações de peso e carregamento.

Outro ponto observado foi em relação às URLs de redirecionamento, que apresentavam erro. No entanto, considerei que isso não impactaria o desenvolvimento técnico do teste, pois os links funcionam como placeholders estruturais.

Durante a implementação, enfrentei alguns desafios específicos:

- Alinhamento na seção "New Arrivals":

Inicialmente tive dificuldade para posicionar o preço e o botão lado a lado. A solução foi estruturar ambos dentro de uma <table> com <td> separados, garantindo alinhamento consistente entre os elementos.

- Construção do banner com botões:

Minha primeira abordagem foi utilizar background-image com botões sobrepostos. No entanto, ao pesquisar mais profundamente, identifiquei limitações dessa técnica em clientes de e-mail.

Diante disso, considerei duas alternativas:

1 - Utilizar VML (especialmente para Outlooks);
2 - Fatiar a imagem em múltiplas partes.

Optei pela segunda abordagem, por ser a mais simples e amplamente compatível. Para isso, utilizei o Figma para dividir o banner em seções, incluindo partes com botões incorporados. Em seguida, montei a estrutura utilizando tabelas, onde cada linha representava uma parte da imagem, aplicando links nas áreas correspondentes.

- Construção das linhas decorativas no rodapé:

Para replicar o layout proposto, utilizei uma combinação de <td> com altura mínima e border-top em tabelas subsequentes, garantindo fidelidade visual ao design original.

De forma geral, considerei o desenvolvimento mais fluido do que o esperado. O desafio foi bastante enriquecedor, proporcionando aprendizado prático sobre boas práticas em e-mail marketing, além de reforçar a importância de adaptação técnica conforme o contexto da aplicação.


Referências de estudo utilizadas:

https://designmodo.com/html-css-emails/

https://www.godaddy.com/resources/br/artigos/regras-para-envio-de-e-mail-marketing

https://webdesign.tutsplus.com/pt/build-an-html-email-template-from-scratch--webdesign-12770a

https://www.hostgator.com.br/blog/hml-email-marketing/

https://oglobo.globo.com/projetos/midiakit-specs/assets/boaspraticas.pdf