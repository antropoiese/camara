<strong>Documantação do projeto</strong>

O objetivo inicial do projeto era desenvolver visualizações de dados que permitissem identificar padrões de comportamento de parlamentares mulheres, bem como do corpo total de parlamentares em relação à questões de gênero. Para tanto, pretendíamos analisar  um recorte de votações "emblemáticas" de proposições referentes à questões de gênero. A ideia era explorar diversas possibilidades, como o posicionamento das legendas e d@s parlamentares individualmente, focando, principalmente, no comportamento das parlamentares mulheres.

Com isso, esperávamos gerar uma maior compreensão sobre a dinâmica da representação de mulheres no parlamento, contribuindo com o fortalecimento da democracia e a ampliação da participação da sociedade civil na tomada de decisões do Congresso Nacional. A visualização de dados sobre o comportamento das parlamentares mulheres que compõem o Congresso Nacional, bem como do corpo completo de parlamentares em relação às propostas que relacionam-se com questões de gênero, permitiria aumentar o controle social sobre @s representantes, buscando compreender possíveis diferenças no comportamento d@s parlamentares. Acreditamos que estudos dessa natureza podem auxiliar na compreensão da dinâmica da representação (ou subrepresentação?) das mulheres no Congresso, auxiliando na formulação de políticas afirmativas e no accoutability de todo o corpo de parlamentares.

No primeiro dia de trabalho, nos deparamos com um primeiro obstáculo: as votações selecionadas (importantes leis aprovadas em plenário relacionadas a questão de gênero) apresentavam poucos votos contrários e as orientações partidárias eram praticamente unânimes pela aprovação dos projetos. O padrão nos sugere que, ao chegar ao plenário, as proposições já contam com uma articulação favorável à sua aprovação. Passamos então a buscar proposições relacionadas à temas mais sensíveis, como aborto. Apesar de haverem diversas propostas que pretendam regular a questão, nenhuma delas chegou ao plenário em período recente. Isso sugere que, em sua maioria, essas proposições são barradas dentro das comissões temáticas por onde tramitam, de modo que jamais se constitue um cenário favorável à sua aprovação, ou seja, elas nunca são levadas a plenário O dado reforça a percepção de que uma análise das votações em plenário contribuiria pouco para identificar padrões de comportamentos n@s parlamentares, tendo em vista que a maioria se atém as articulações prévias que determinam as posições das bancadas. 

Seria necessário, então buscar formas de compreender como se dava o processo de discussão e votação dentro das comissões. O desafio, entretanto, é que o regulamento da Câmara permite votações nominais dentro das comissões. As votações nominais não são convertidas em dados que alimentem o sistema de dados abertos da Câmara. Ou seja: apesar da lei da transparência, a própria dinâmica de funcionamento da casa legislativa dificulta o monitoramento do comportamento d@s parlamentares para aprovar ou derrubar uma proposição antes que ela chegue ao Plenário. 

Optamos então por seguir um caminho diferente, que nos permitisse alcançar um resultado próximo daquele aspirado inicialmente. A solução foi analisar, a partir do sistema de indexação da Câmara, que utiliza palavras-chave para segmentar por temas as proposições , os principais temas das proposições de parlamentares mulheres nas legislaturas recentes. 


<strong>Documentação do Projeto Dinâmica da Participação Feminina no Congresso</strong>

Dinâmica da Participação Feminina no Congresso é  uma aplicação web que permite a todos os cidadãos conhecerem os temas mais enfatizados pelas Deputadas Federais em suas proposições.
A análise tem como recorte a 54ª legislatura (2011-2014) e considerou as 801 proposições de 46  deputadas. Observamos a indexação das proposições para identificar os principais temas sobre os quais se propõem a legislar. 

<strong>Motivação</strong>

O objetivo do projeto é auxiliar a compreensão da dinâmica da representação (ou subrepresentação?) das mulheres no Congresso, fomentando o debate a cerca da formulação de políticas afirmativas e o accoutability de todo o corpo de parlamentares. 

Optamos por desenvolver visualizações de dados que permitam identificar não apenas a presença feminina na câmara dos deputados, mas também padrões temáticos de suas proposições, oferecendo um panorama de caráter mais qualitativo da atuação destas mulheres, identificando padrões temáticos das proposições que apresentam. 

Também buscamos explorar outras possibilidades, como a presença de parlamentares mulheres nas bancadas partidárias, fomentando um debate sobre a participação das mulheres na política pela perspectiva da presença nos partidos. 

<strong>Metodologia</strong>

A metodologia de desenvolvimento do trabalho seguiu três etapas básicas:

<strong>Obtenção dos dados</strong>

Os dados foram obtidos por meio da API disponível nos <a href='http://www2.camara.leg.br/transparencia/dados-abertos/dados-abertos-legislativo'>Dados Abertos</a> da Câmara dos Deputados. Foram coletadas todas as proposições de projetos de lei com autoras do sexo femininos na 54ª legislatura bem como dados de todos os deputados e deputados eleitos na atual legislatura.

<strong>Limpeza, tratamento e organização dos dados</strong>

Os dados dos deputados e das deputadas eleitos na atual legislatura bem como os dados dos projetos de lei propostos pelas deputadas foram tratados de modo a poderem ser visualizados em forma de <a href='http://pt.wikipedia.org/wiki/Teoria_dos_grafos'>grafos</a>. 

<strong>Visualização</strong>

Para a visualização dos dados em formato de grafo utilizou-se o software <a href='http://gephi.github.io/'>Gephi</a> com o plugin <a href='https://marketplace.gephi.org/plugin/circular-layout/'>Circular Layout</a>. Os arquivo tratados no Gephi foram exportados em formato *.gexf e então utilizou-se o plugin <a href='https://marketplace.gephi.org/plugin/gexf-js-web-viewer/'>Gexf-JS Web Viewer</a> para visualização em formato *.html. Para a visualização em formato html dos projetos de lei procedeu-se à personalização do plugin Gexf-JS Web Viewer direto no código-fonte em javascript para que a visualização incorporasse, na exibição, links para os projetos de projetos de lei analisados.
