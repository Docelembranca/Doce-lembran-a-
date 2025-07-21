<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Doce Lembrança - Doces Artesanais</title>
  <style>
    /* Reset básico */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: #fff5f7;
      color: #5a2a27;
      line-height: 1.6;
    }

    header {
      background: #f7c6c6;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 3px 6px rgba(0,0,0,0.1);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    header h1 {
      font-family: 'Pacifico', cursive;
      font-size: 2rem;
      color: #a63838;
      letter-spacing: 2px;
    }

    nav a {
      color: #7a2b2b;
      text-decoration: none;
      margin-left: 25px;
      font-weight: 600;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #d64646;
    }

    .banner {
      background: url('https://images.unsplash.com/photo-1551024601-bec78aea704b?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
      height: 350px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      text-shadow: 2px 2px 6px #7a2b2b;
      font-size: 2.8rem;
      font-weight: bold;
      font-family: 'Pacifico', cursive;
      letter-spacing: 3px;
    }

    main {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }

    section {
      margin-bottom: 50px;
    }

    h2 {
      color: #a63838;
      margin-bottom: 25px;
      font-size: 2rem;
      border-bottom: 3px solid #d64646;
      display: inline-block;
      padding-bottom: 5px;
    }

    /* Produtos doces */
    .produtos {
      display: flex;
      flex-wrap: wrap;
      gap: 25px;
      justify-content: center;
    }

    .produto {
      background: #fff0f3;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(166,54,54,0.2);
      width: 280px;
      padding: 15px;
      text-align: center;
      transition: transform 0.3s ease;
      cursor: pointer;
    }

    .produto:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 15px rgba(166,54,54,0.35);
    }

    .produto img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 15px;
    }

    .produto h3 {
      color: #7a2b2b;
      margin-bottom: 10px;
      font-size: 1.3rem;
    }

    .produto p {
      font-size: 0.95rem;
      color: #5a2a27;
    }

    /* Sobre */
    .sobre p {
      max-width: 700px;
      font-size: 1.1rem;
      color: #633535;
    }

    /* Contato */
    form {
      max-width: 500px;
      background: #fff0f3;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(166,54,54,0.2);
    }

    form label {
      display: block;
      margin-bottom: 8px;
      font-weight: 600;
      color: #7a2b2b;
    }

    form input, form textarea {
      width: 100%;
      padding: 10px 12px;
      margin-bottom: 18px;
      border: 2px solid #d64646;
      border-radius: 6px;
      font-size: 1rem;
      font-family: inherit;
      resize: vertical;
    }

    form button {
      background: #a63838;
      color: white;
      border: none;
      padding: 12px 25px;
      font-size: 1rem;
      font-weight: 700;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    form button:hover {
      background: #d64646;
    }

    footer {
      background: #f7c6c6;
      padding: 20px 40px;
      text-align: center;
      color: #7a2b2b;
      font-weight: 600;
      font-size: 0.9rem;
    }

    /* Responsividade */
    @media (max-width: 768px) {
      .produtos {
        flex-direction: column;
        align-items: center;
      }

      header {
        flex-direction: column;
        gap: 10px;
        padding: 20px;
      }

      nav a {
        margin-left: 0;
        margin-right: 20px;
      }
    }
  </style>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet" />
</head>
<body>
  <header>
    <h1>Doce Lembrança</h1>
    <nav>
      <a href="#produtos">Produtos</a>
      <a href="#sobre">Sobre</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <div class="banner">
    Doces que fazem você sorrir
  </div>

  <main>
    <section id="produtos">
      <h2>Nossos Doces</h2>
      <div class="produtos">
        <div class="produto">
          <img src="https://images.unsplash.com/photo-1562440499-d42f87b85b18?auto=format&fit=crop&w=400&q=80" alt="Brigadeiro tradicional" />
          <h3>Brigadeiro Tradicional</h3>
          <p>O clássico doce brasileiro, cremoso e irresistível.</p>
        </div>
        <div class="produto">
          <img src="https://images.unsplash.com/photo-1562440498-5e6e3a5b1f97?auto=format&fit=crop&w=400&q=80" alt="Beijinho" />
          <h3>Beijinho</h3>
          <p>Delicado doce de coco com toque de leite condensado.</p>
        </div>
        <div class="produto">
          <img src="https://images.unsplash.com/photo-1505253210343-1f858b41c68a?auto=format&fit=crop&w=400&q=80" alt="Cupcake de baunilha" />
          <h3>Cupcake de Baunilha</h3>
          <p>Fofo e saboroso, perfeito para qualquer ocasião.</p>
        </div>
      </div>
    </section>

    <section id="sobre" class="sobre">
      <h2>Sobre Nós</h2>
      <p>
        Na Doce Lembrança, acreditamos que doces são mais do que sobremesas — são momentos de felicidade que ficam guardados na memória. Todos os nossos produtos são feitos artesanalmente com ingredientes selecionados para garantir sabor e qualidade.
      </p>
    </section>

    <section id="contato">
      <h2>Contato</h2>
      <form>
        <label for="nome">Nome</label>
        <input type="text" id="nome" name="nome" placeholder="Seu nome" required />

        <label for="email">Email</label>
        <input type="email" id="email" name="email" placeholder="seu@email.com" required />

        <label for="mensagem">Mensagem</label>
        <textarea id="mensagem" name="mensagem" rows="4" placeholder="Escreva sua mensagem..." required></textarea>

        <button type="submit">Enviar</button>
      </form>
    </section>
  </main>

  <footer>
    &copy; 2025 Doce Lembrança — Feito com carinho 💖
  </footer>
</body>
</html>

