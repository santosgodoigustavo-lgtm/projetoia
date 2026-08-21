# projetoia
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AURA | Loja de Roupas & Moda</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Helvetica Neue', Arial, sans-serif;
        }

        :root {
            --primary: #111111;
            --accent: #d90429;
            --gray-light: #f4f4f6;
            --text-dark: #2b2d42;
        }

        body {
            background-color: #ffffff;
            color: var(--text-dark);
            line-height: 1.5;
        }

        /* BANNER TOPO */
        .top-bar {
            background-color: var(--primary);
            color: #ffffff;
            text-align: center;
            padding: 8px;
            font-size: 0.85rem;
            letter-spacing: 1px;
        }

        /* NAVEGAÇÃO */
        header {
            border-bottom: 1px solid #e5e5e5;
            position: sticky;
            top: 0;
            background: #ffffff;
            z-index: 100;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 18px 20px;
        }

        .brand-logo {
            font-size: 1.8rem;
            font-weight: 900;
            letter-spacing: 3px;
            color: var(--primary);
            text-decoration: none;
        }

        .menu {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .menu a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            transition: color 0.2s;
        }

        .menu a:hover {
            color: var(--accent);
        }

        /* CAPA (HERO) */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://encrypted-tbn0.gstatic.com/licensed-image?q=tbn:ANd9GcRZLSk1qRZUnsz7Omb99UsuZSl8Og2mTnf9TDP78sfE2NGprr3LzaJ6d0wX-kqMlp5NdQ4V2bNHImTm1IA') center/cover no-repeat;
            height: 480px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #ffffff;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 15px;
            text-transform: uppercase;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 25px;
            font-weight: 300;
        }

        .btn-banner {
            background-color: #ffffff;
            color: var(--primary);
            padding: 12px 30px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 4px;
            text-transform: uppercase;
            transition: background 0.3s;
        }

        .btn-banner:hover {
            background-color: var(--accent);
            color: #ffffff;
        }

        /* SEÇÃO DE PRODUTOS */
        .products-section {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .title-section {
            text-align: center;
            font-size: 1.8rem;
            margin-bottom: 40px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: #ffffff;
            border-radius: 8px;
            overflow: hidden;
            border: 1px solid #efefef;
            transition: transform 0.2s, box-shadow 0.2s;
            display: flex;
            flex-direction: column;
        }

        .product-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.08);
        }

        .product-img {
            width: 100%;
            height: 340px;
            object-fit: cover;
            background-color: #f8f8f8;
        }

        .product-details {
            padding: 20px;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .product-name {
            font-size: 1.05rem;
            margin-bottom: 8px;
            color: var(--primary);
        }

        .product-price {
            font-size: 1.3rem;
            font-weight: bold;
            color: var(--accent);
            margin-bottom: 15px;
        }

        .btn-buy {
            background-color: var(--primary);
            color: #ffffff;
            border: none;
            padding: 12px;
            border-radius: 4px;
            font-weight: bold;
            cursor: pointer;
            width: 100%;
            margin-top: auto;
            transition: background 0.2s;
        }

        .btn-buy:hover {
            background-color: #333333;
        }

        /* INFORMAÇÕES DE COMPRA */
        .benefits {
            background-color: var(--gray-light);
            padding: 40px 20px;
            margin-top: 60px;
        }

        .benefits-grid {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            text-align: center;
        }

        .benefit-box h3 {
            font-size: 1rem;
            margin-bottom: 5px;
        }

        .benefit-box p {
            font-size: 0.9rem;
            color: #666;
        }

        /* RODAPÉ */
        footer {
            background-color: var(--primary);
            color: #ffffff;
            text-align: center;
            padding: 25px 20px;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <div class="top-bar">
        FRETE GRÁTIS PARA TODO O BRASIL EM COMPRAS ACIMA DE R$ 299
    </div>

    <header>
        <div class="nav-container">
            <a href="#" class="brand-logo">AURA</a>
            <ul class="menu">
                <li><a href="#lançamentos">Lançamentos</a></li>
                <li><a href="#feminino">Feminino</a></li>
                <li><a href="#masculino">Masculino</a></li>
            </ul>
        </div>
    </header>

    <section class="hero">
        <div>
            <h1>Nova Coleção 2026</h1>
            <p>Roupas exclusivas projetadas para conforto e estilo urbano.</p>
            <a href="#produtos" class="btn-banner">Confira as Peças</a>
        </div>
    </section>

    <main class="products-section" id="produtos">
        <h2 class="title-section">Destaques da Loja</h2>

        <div class="product-grid">
            <!-- Produto 1 -->
            <div class="product-card">
                <img src="https://encrypted-tbn0.gstatic.com/licensed-image?q=tbn:ANd9GcRZLSk1qRZUnsz7Omb99UsuZSl8Og2mTnf9TDP78sfE2NGprr3LzaJ6d0wX-kqMlp5NdQ4V2bNHImTm1IA" alt="Vestido Elegante Vermelho" class="product-img">
                <div class="product-details">
                    <h3 class="product-name">Vestido Gala Vermelho</h3>
                    <p class="product-price">R$ 299,90</p>
                    <button class="btn-buy">Adicionar ao Carrinho</button>
                </div>
            </div>

            <!-- Produto 2 -->
            <div class="product-card">
                <img src="https://s2.javalicouros.com.br/product/2024/12/730-vest-preto-4.jpg" alt="Jaqueta de Couro Masculina" class="product-img">
                <div class="product-details">
                    <h3 class="product-name">Jaqueta Couro Biker</h3>
                    <p class="product-price">R$ 459,00</p>
                    <button class="btn-buy">Adicionar ao Carrinho</button>
                </div>
            </div>

            <!-- Produto 3 -->
            <div class="product-card">
                <img src="https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcQ-g73Ugsb6vjngZgBCdLUrGcyub9pGBr0g-kmu5VvjB2_RxV5IqROOUw4tWnC_VCKkpwEClmD3enkl9ro" alt="Conjunto Verão Básico" class="product-img">
                <div class="product-details">
                    <h3 class="product-name">Conjunto Verão Linho</h3>
                    <p class="product-price">R$ 189,90</p>
                    <button class="btn-buy">Adicionar ao Carrinho</button>
                </div>
            </div>
        </div>
    </main>

    <section class="benefits">
        <div class="benefits-grid">
            <div class="benefit-box">
                <h3>Envio Rápido</h3>
                <p>Despachamos em até 24h úteis</p>
            </div>
            <div class="benefit-box">
                <h3>Troca Garantida</h3>
                <p>30 dias sem custo adicional</p>
            </div>
            <div class="benefit-box">
                <h3>Parcele em 6x</h3>
                <p>Sem juros no cartão de crédito</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 AURA Moda. Todos os direitos reservados.</p>
    </footer>

</body>
</html>