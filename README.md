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
    <footer>
        <p>&copy; 2025 Portal dos Jogos</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background: #ffe6f7;
    color: #7b2869;
    margin: 0;
    padding: 0;
}
header {
    background: #ff69b4;
    padding: 20px 0;
    text-align: center;
}
header h1 {
    margin: 0;
    color: #fff;
}
nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0 0;
}
nav ul li {
    display: inline-block;
    margin: 0 15px;
}
nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
}
main {
    padding: 30px;
}
section {
    margin-bottom: 40px;
}
h2 {
    color: #e43f6f;
    border-bottom: 2px solid #ffb6d5;
    padding-bottom: 5px;
}
.jogos-lista, .categorias-lista {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
}
.jogos-lista article, .categorias-lista > div {
    background: #ffd6ef;
    border-radius: 12px;
    padding: 18px;
    flex: 1 1 200px;
    min-width: 220px;
    box-shadow: 0 2px 8px #f8a5c2;
}
.jogos-lista img {
    width: 100%;
    border-radius: 8px;
    margin-bottom: 10px;
}
footer {
    background: #ff69b4;
    color: #fff;
    text-align: center;
    padding: 15px 0;
    margin-top: 30px;
}
form {
    background: #ffd6ef;
    padding: 16px;
    border-radius: 10px;
    margin-bottom: 20px;
    max-width: 400px;
}
form label {
    display: block;
    margin-top: 10px;
    color: #7b2869;
}
form input, form textarea {
    width: 100%;
    padding: 8px;
    margin-top: 5px;
    border: 1px solid #e43f6f;
    border-radius: 6px;
    font-size: 1em;
    background: #fff;
    color: #7b2869;
}
form button {
    margin-top: 15px;
    background: #e43f6f;
    color: #fff;
    border: none;
    padding: 10px 18px;
    border-radius: 6px;
    cursor: pointer;
    font-weight: bold;
    transition: background 0.2s;
}
form button:hover {
    background: #c2185b;
}
#listaComentarios {
    max-width: 500px;
}
.comentario {
    background: #fff0fa;
    border: 1px solid #e43f6f;
    border-radius: 8px;
    padding: 10px;
    margin-bottom: 10px;
}
.comentario strong {
    color: #e43f6f;
}
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
