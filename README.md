# Entrega 1 (NÃO É PRA ENVIAR ESSE PRA PROFESSORA)

## 🧠 Etapas para Desenvolver o Projeto

### 1. *Modelagem das Classes*
Comece com o esqueleto das principais classes:

| Classe         | Atributos principais                          | Métodos sugeridos                          |
|----------------|-----------------------------------------------|--------------------------------------------|
| Usuario      | nome, email, playlists                        | criarPlaylist(), removerPlaylist(), etc.   |
| Midia (abstract) | título, artista, duração, gênero         | getters/setters                            |
| Musica, Podcast, Audiobook | herdam de Midia         | podem ter atributos extras (ex: narrador)  |
| Playlist     | nome, lista de mídias                         | adicionarMidia(), removerMidia(), calcularDuracao() |
| Catalogo     | lista ou mapa de mídias                       | buscarPorTitulo(), buscarPorArtista(), buscarPorGenero() |
| Genero (enum)| ROCK, POP, MPB, JAZZ, CLASSICA...             | —                                          |

Use *herança* para Midia e suas subclasses, *polimorfismo* para tratar diferentes tipos de mídia, e *encapsulamento* para proteger os dados.

---

### 2. *Estrutura de Dados*
- Use List<Midia> para playlists.
- Use Map<String, Midia> ou Set<Midia> para o catálogo.
- Pode usar Map<Usuario, List<Playlist>> se quiser centralizar tudo.

---

### 3. *Tratamento de Exceções*
Crie exceções personalizadas como:
java
public class MidiaNaoEncontradaException extends Exception {
    public MidiaNaoEncontradaException(String mensagem) {
        super(mensagem);
    }
}

Use try-catch ao buscar mídias ou manipular playlists.

---

### 4. *Fluxo Básico*
1. Cadastro de usuários.
2. Cadastro de mídias no catálogo.
3. Criação de playlists.
4. Adição/remoção de mídias.
5. Visualização de playlists.
6. Busca no catálogo.

---

### 5. *Análise Crítica com ChatGPT*
Depois de implementar, peça pra eu gerar uma versão alternativa do projeto. Aí vocês comparam:

- Estrutura de classes
- Uso de herança/polimorfismo
- Escolha de coleções
- Clareza e organização
- Tratamento de erros

Dá pra fazer uma tabela comparativa com prós e contras de cada abordagem.

---
