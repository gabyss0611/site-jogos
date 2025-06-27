<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Portal dos Jogos</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Portal dos Jogos</h1>
        <p class="descricao-site">Site criado por <strong>gabys dele</strong> - Seu portal para jogos de todos os tipos, com alta qualidade!</p>
        <nav>
            <ul>
                <li><a href="#destaques">Destaques</a></li>
                <li><a href="#categorias">Categorias</a></li>
                <li><a href="#quebracabeca">Quebra-Cabeça</a></li>
                <li><a href="#comentarios">Comentários</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="destaques">
            <h2>Jogos em Destaque (Alta Qualidade)</h2>
            <div class="jogos-lista">
                <article>
                    <h3>The Witcher 3: Wild Hunt</h3>
                    <img src="https://upload.wikimedia.org/wikipedia/en/0/0c/Witcher_3_cover_art.jpg" alt="Capa The Witcher 3">
                    <p>Jogo de RPG aclamado mundialmente, com gráficos incríveis e história envolvente.</p>
                </article>
                <article>
                    <h3>God of War</h3>
                    <img src="https://upload.wikimedia.org/wikipedia/pt/a/a7/God_of_War_4_capa.png" alt="Capa God of War">
                    <p>Ação, aventura e uma jornada épica baseada na mitologia nórdica.</p>
                </article>
            </div>
        </section>
        <section id="categorias">
            <h2>Jogos por Categoria</h2>
            <div class="categorias-lista">
                <div>
                    <h3>Ação</h3>
                    <ul>
                        <li>Call of Duty</li>
                        <li>Fortnite</li>
                        <li>Grand Theft Auto V</li>
                    </ul>
                </div>
                <div>
                    <h3>Aventura</h3>
                    <ul>
                        <li>Uncharted 4</li>
                        <li>Assassin's Creed Odyssey</li>
                        <li>Red Dead Redemption 2</li>
                    </ul>
                </div>
                <div>
                    <h3>Esportes</h3>
                    <ul>
                        <li>FIFA 24</li>
                        <li>NBA 2K25</li>
                        <li>eFootball</li>
                    </ul>
                </div>
                <div>
                    <h3>Corrida</h3>
                    <ul>
                        <li>Forza Horizon 5</li>
                        <li>Gran Turismo 7</li>
                        <li>Mario Kart 8</li>
                    </ul>
                </div>
            </div>
        </section>
        <section id="quebracabeca">
            <h2>Jogos de Quebra-Cabeça</h2>
            <div class="jogos-lista">
                <article>
                    <h3>Portal 2</h3>
                    <img src="https://upload.wikimedia.org/wikipedia/en/3/3d/Portal2cover.jpg" alt="Capa Portal 2">
                    <p>Desafie sua mente resolvendo enigmas usando portais!</p>
                </article>
                <article>
                    <h3>Tetris Effect</h3>
                    <img src="https://upload.wikimedia.org/wikipedia/en/2/2a/Tetris_Effect_cover_art.jpg" alt="Capa Tetris Effect">
                    <p>O clássico Tetris com gráficos e trilha sonora incríveis.</p>
                </article>
            </div>
        </section>
        <section id="comentarios">
            <h2>Comentários</h2>
            <form id="comentarioForm">
                <label for="nome">Nome:</label>
                <input type="text" id="nome" name="nome" required>
                <label for="mensagem">Mensagem:</label>
                <textarea id="mensagem" name="mensagem" required></textarea>
                <button type="submit">Enviar Comentário</button>
            </form>
            <div id="listaComentarios">
                <!-- Comentários aparecerão aqui -->
            </div>
        </section>
    </main>
    body {
    font-family: Arial, sans-serif;
    background: #181818;
    color: #f4f4f4;
    margin: 0;
    padding: 0;
}
header {
    background: #262626;
    padding: 20px 0;
    text-align: center;
}
header h1 {
    margin: 0;
}
nav ul {
    list-style: none;
    padding: 0;
}
nav ul li {
    display: inline-block;
    margin: 0 15px;
}
nav ul li a {
    color: #ffd700;
    text-decoration: none;
    font-weight: bold;
}
main {
    padding: 30px;
}
section {
    margin-bottom: 40px;
}
article {
    background: #222;
    border-radius: 8px;
    padding: 15px;
    margin-bottom: 15px;
}
footer {
    background: #262626;
    text-align: center;
    padding: 15px 0;
    margin-top: 30px;
}
    <footer>
        <p>&copy; 2025 Portal dos Jogos</p>
    </footer>
    <script src="script.js"></script>
</body>
</html># site-jogos
document.getElementById('comentarioForm').addEventListener('submit', function(event) {
    event.preventDefault();
    const nome = document.getElementById('nome').value.trim();
    const mensagem = document.getElementById('mensagem').value.trim();
    if (nome && mensagem) {
        adicionarComentario(nome, mensagem);
        document.getElementById('comentarioForm').reset();
    }
});

function adicionarComentario(nome, mensagem) {
    const lista = document.getElementById('listaComentarios');
    const div = document.createElement('div');
    div.className = 'comentario';
    div.innerHTML = `<strong>${nome}</strong>: ${mensagem}`;
    lista.prepend(div);
}
