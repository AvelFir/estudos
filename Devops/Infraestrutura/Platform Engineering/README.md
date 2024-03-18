
# Platform Engineering

- É o desenho e construçao de ferramentas e workflows que automatizam as necessidades de engenharia de software  na era da cloud, cobrindo todas as necessidades do lifecycle de uma aplicaçao.
- Tambem chamado de Internal Developer Platform (IDP) compreende uma variedade de tecnologias e ferramentas, integradas de maneira que reduzam a carga cognitiva dos desenvolvedores para que eles possam focar no essencial.
- Atuar como um self-service de serviços de plataforma.
- Ajuda a prevenir as armadilhas atuais da realidade Devops


## Pros e Contras

Pros:

- As vantagens para os times de operaçoes é que eles nao precisam mais se preocupar com chamados para a equipe de sys-ops, e podem focar esse tempo em estrategias de iniciativa e as entregas ficam mais seguras, as metricas melhoram pois os erros diminuem.
- As vantagens para os times de desenvolvedores é que eles podem fazer entregas mais rapidas, sem falar com as equipes de sysops, e podem facilmente fazer alteraçoes necessarias no ambiente, implementar apps e recursos, sem a necessidade de saber as tecnologias por tras daquilo, tambem nao precisam se preocupar em criar e manter as infraestruras necessarias para as apps.

Contras:

- Um dos maiores desafios das IDP é nao terem uma boa forma de feedback estruturada e nao ouvirem as melhorias sugeridas
- Falta de personalizaçao
- Forçar os desenvolvedores a adaptar o desenvolvimento, limitando a criatividade.  

## Estabilidade X Inovaçao

- Devemos reconhecer a necessidade da inovaçao, nao apenas busca-la sem motivo, mas entender o que trazemos junto com ela, a tecnologia vem avançando por si so,as regras de negocio ficam mais complexas e os usuarios exigem mais, porem por mais que uma tecnologia nova traga novas funcionalidades ou uma nova performance, devemos levar em consideraçao que tambem estamos abrindo margem para riscos nao conhecidos, falhas em potenciais etc.
- Estabilidade é o sangue de uma plataforma, pois uma plataforma estavel em operaçoes previsiveis e confiaveis sao criticas para o negocio., enquanto inovaçao garante crescimento, estabilidade garante sobrevivencia.
- Estabilidade de plataforma nao se trata apenas de uptime, mas tambem de performance, segurança e previsibilidade.
- Como podemos balancear entre inovaçao e estabilidade?
  - **Prudencia na hora da adoçao:** Nem toda nova tecnologia deve ser adotada de primeira, os beneficios devem ser calculados sobre os riscos, devemos considerar a maturidade da tecnologia e sua curva de aprendizado.
  - **Transiçao Gradual:** Mudanças BigBang raramente sao uma boa ideia, opte por fazer transaçoes graduais de pouco em pouco e pequenas para poder controlar os riscos. 
  - **Aprender e se adaptar:** Quando adotar uma nova tecnlogia aprenda tudo que puder sobre ela, quando uma falha ocorrer aprenda com ela e use para melhorar mais pra frente.

## Liberdade e controle
- O maior beneficio do IDP é o desenvolvedor nao ter que se preocupar com infraestrutura, e poder focar inteiramente em codigo.
- Porem devemos dar liberade ao dev de fazer alteraçoes necessarias nos fluxos, ou oferecer diversos fluxos diversificados para que nao afetamos a criatividade do dev, ou que ele fique preso em fazer soluçoes nao viaveis apenas para atender as demandas da infraestrurua.
- Porem essa liberade deve ser controlada atraves de um time de governança para que existam padraos minimos de qualidade em cada projeto para facilitar o aprendizado e a integraçao.

## Comparando IDP e Abordagens Tradicionais
- Abordagem Tradicional: Envolve muitos anos de pratica de configuraçao e a criaçao de scripts simples para automatizar tarefas. Dessa forma o desenvolvedor provavelmente possui muitos scripts prontos para lhe auxiliarem, e permite uma personalizaçao completa, que frequentemente nao é possivel nos IDPs. Porem isso faz com que percam muito tempo configurando ou ate criando os scripts.
- IDP: Podem salvar muito tempo de produtivivade pois busca simplificar e automatizar muitas configuraçoes que o desenvolvedor iria ter que fazer, entretando implementa-la é complexo e nao podemos esquecer que ela nao garante uma boa flexibilidade quando for necessario fazer alteraçoes, fazendo com que em casos especificos o desenvolvedor tenha que fazer a configuraçao por fora da plataforma.

## Links
* https://platformengineering.org/blog/what-is-platform-engineering
* https://www.stackspot.com/en/blog/innovation-and-stability-in-platform-teams
* https://www.stackspot.com/en/blog/freedom-and-control-in-using-internal-developer-platforms
* https://www.stackspot.com/en/blog/comparing-internal-developer-platforms
* https://humanitec.com/blog/spotify-backstage-service-catalog
* https://docs.stackspot.com/en/home/stackspot/getting-started/