## Descrição das Classes

**Usuário:** representa uma pessoa que pode acessar o sistema. Ela reúne os atributos e comportamentos comuns aos diferentes tipos de usuários, evitando duplicação de código. Por ser uma classe abstrata, ela não pode ser instanciada diretamente, servindo apenas como base para outras classes.

**Jogador:** Representa os atletas pertencentes às seleções participantes da Copa do Mundo. Cada jogador pertence a uma única seleção e pode participar de diversas partidas durante a competição.

**Técnico:** Representa o treinador responsável por comandar uma seleção. Cada seleção possui apenas um técnico responsável.

**Seleção:** Representa uma seleção nacional participante da Copa do Mundo. A seleção reúne seus jogadores, possui um técnico responsável e participa das partidas do torneio.

**Grupo:** Representa os grupos da fase inicial da Copa do Mundo. Cada grupo reúne diversas seleções que disputam vagas para a fase eliminatória.

**Partida:** Representa um jogo realizado durante a competição. Cada partida ocorre em um estádio específico, envolve exatamente duas seleções e gera um conjunto de estatísticas.

**Estádio:** Representa os estádios utilizados durante a competição. Um estádio pode receber diversas partidas ao longo da competição.

**Estatística:** Representa as estatísticas produzidas durante uma partida. Cada objeto de estatística está diretamente relacionado a uma única partida.

## Justificativa dos Relacionamentos

### Herança:

**Usuário \<- Jogador**

**Usuário \<- Técnico**

Foi utilizada herança porque **jogadores e técnicos** possuem informações em comum, como nome, e-mail, senha e telefone. Esses atributos e comportamentos foram centralizados na classe abstrata **Usuário**.

### Agregação:

**Agregação entre Grupo e Seleção:** Foi utilizada agregação porque um grupo é formado por diversas seleções, porém as seleções possuem existência independente. Mesmo que uma seleção deixe de pertencer a um determinado grupo, ela continua existindo no sistema.

**Agregação entre Partida e Seleção:** A agregação representa que uma partida envolve exatamente duas seleções participantes. Entretanto, as seleções existem independentemente da partida e podem participar de diversos jogos durante a competição.

### Composição:

**Composição entre Seleção e Jogador:** Foi utilizada composição porque os jogadores fazem parte da estrutura da seleção dentro do contexto do sistema. A seleção é responsável por manter sua lista de jogadores, caracterizando uma relação de todo-parte.

**Composição entre Seleção e Técnico:** Cada seleção possui exatamente um técnico responsável. O técnico faz parte da composição da equipe técnica da seleção, justificando o uso da composição.

**Composição entre Partida e Estatística:** A composição foi utilizada porque as estatísticas existem exclusivamente para registrar os dados de uma determinada partida. Caso a partida deixe de existir, suas estatísticas também deixam de fazer sentido, caracterizando uma relação de dependência forte.

### Associação:

**Associação entre Partida e Estádio:** Cada partida acontece em um estádio específico. O estádio existe independentemente das partidas, sendo apenas utilizado como local de realização dos jogos.

**Associação entre Jogador e Partida:** Foi utilizada uma associação muitos-para-muitos, pois um jogador pode disputar várias partidas ao longo da competição e cada partida possui diversos jogadores participantes.

