# Projetando Pokemon BD - I DSN

![pokemon](https://t.ctcdn.com.br/IZbPIPMfS8TzOqMQJthZUo4cTMg=/1024x576/smart/i515431.jpeg)

Exemplo de 1 pokemon : https://wiki.otpokemon.com/index.php/Abra

Neste jogo de pokemons, vamos precisar armazenar alguns dados importantes para manter a jogabilidade adequada.

Este jogo funciona da seguinte maneira:

O jogo gira em torno de Pokemons, portanto precisaremos armazenar alguns dados sobre eles. Cada Pokémon deve ser identificado por um número único chamado ID_Pokemon, e cada pokemon deve ter um nome exclusivo. Além disso, é necessário registrar o [ tipo primário](https://pokemon.fandom.com/pt-br/wiki/Tipo) do Pokémon, bem como suas habilidades especiais. O nível de evolução do Pokémon deve ser registrado, assim como a altura e o peso do Pokémon.

É importante armazenar também de maneira detalhada os [tipos](https://pokemon.fandom.com/pt-br/wiki/Tipo). Cada tipo deve ter um identificador único chamado ID_Tipo, um nome e uma descrição que explica as características do tipo. Um Pokémon deve ter obrigatoriamente 1 ou mais tipos associados a ele. Um tipo pode ser criado sem nenhum Pokémon estar associado a ele. Um tipo pode estar associado para mais de 1 Pokémon.

Assim como os tipos, precisaremos guardar as [habilidades](https://wiki.otpokemon.com/index.php/Habilidades_dos_Pokemon). Cada habilidade deve ter um identificador único chamado ID_Habilidade, um nome e uma descrição detalhada. Um pokemon pode ter no mínimo uma habilidade. Uma habilidade pode existir sem ter um pokemon associado, porém nada impede de muitos pokemons terem a mesma habilidade.

Os treinadores devem ser identificados por um número único chamado ID_Treinador e devem ter um nome, idade e endereço completo. Um treinador pode treinar muitos pokemons, contudo devemos ter em mente que um treinador novo pode demorar para encontrar seu primeiro pokemon. Um pokemon pode existir sem estar sendo treinado por alguém, isso quer dizer que ele pode não ter sido capturado ainda. Ao ser capturado ele só poderá ter 1 único treinador.

Cada batalha deve ser registrada com um identificador único denominado ID_Batalha, e deve incluir a data da batalha. O treinador participa da batalha, com isto devemos guardar seu ID no registro da batalha. O pokemon luta a batalha, dessa forma deve-se registrar o ID_Pokemon usado por cada treinador. O resultado da batalha deve ser registrado, isto é, mostrar a pontuação (1 x 0, 3 x 9, etc), além disso deve-se registrar o Pokémon vencedor.
