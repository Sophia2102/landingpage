<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page</title>
    <style>
        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            background-color: #f4f4f9;
            color: #000000;
        }
        body::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 300px;
            height: 100%;
            background: url('background-terno.jpg') no-repeat center center;
            background-size: cover;
            opacity: 100;
            z-index: -1;
        }
        header {
            background: linear-gradient(to right, #61ed7f, #00f2fe);
            color: #ffffff;
            padding: 2rem 0;
            text-align: center;
            position: relative;
        }
        header h1 {
            font-size: 2.5rem;
            margin: 0;
            display: inline-block;
        }
        header img {
    width: 250px;
    height: auto;
    vertical-align: middle;
    margin-right: 1rem;
}

        header p {
            font-size: 1.2rem;
            margin-top: 0.5rem;
        }
        nav {
            margin: 1rem auto;
            text-align: center;
        }
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #fff;
            font-weight: bold;
            font-size: 1.1rem;
        }
        nav a:hover {
            text-decoration: underline;
        }
        section {
            padding: 4rem 2rem;
            text-align: center;
        }
        section h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
            color: #333;
        }
        section p {
            font-size: 1.2rem;
            margin: 0 auto 2rem;
            max-width: 600px;
        }
        .cta {
        background: #61ed7f;
        color: #fff;
        padding: 1rem 0;
        border: none;
        border-radius: 50px;
        cursor: pointer;
        font-size: 1.2rem;
        width: 100%; /* Mesma largura do vídeo */
        max-width: 1325px; /* Define um limite máximo */
    
        margin: 1rem auto; /* Centraliza o botão */
        transition: background 0.3s ease;
}
.cta-video {
    background: #61ed7f;
    color: #fff;
    padding: 1rem 0;
    border: none;
    border-radius: 50px;
    cursor: pointer;
    font-size: 1.2rem;
    width: 80%; /* Mesma largura do vídeo */
    max-width: 800px; /* Limite máximo */
    display: block;
    margin: 1rem auto; /* Centraliza o botão */
    transition: background 0.3s ease;
}

.cta-video:hover {
    background: #0056b3;
}


        
        .cta:hover {
            background: #252525;
        }
        video {
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        footer {
            background: #333;
            color: #fff;
            text-align: center;
            padding: 2rem 0;
        }
        footer p {
            margin: 0;
        }
        @media (min-width: 768px) {
            section {
                padding: 4rem 8rem;
            }
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }
        .modal-content {
            background: #fff;
            padding: 2rem;
            border-radius: 8px;
            width: 90%;
            max-width: 400px;
            text-align: left;
        }
        .close {
            float: right;
            font-size: 1.5rem;
            color: #333;
            cursor: pointer;
        }
        .form-group {
            margin-bottom: 1rem;
        }
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
        }
        .form-group input {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <header>
        <img src="aw.png" alt="Logo da Empresa">
       
        <h2><strong>Método Gestão estratégica de pessoas</strong></h2>

    </header>

    <section id="topics">
        <h2>Saiba liderar sua equipe sem dor de cabeça</h2>
        <h1>Assista a aula de introdução gratuitamente e você vai aprender 3 coisas:</h1>
        <div style="padding: 2rem 1rem; text-align: center;">
            <div style="margin-bottom: 2rem;">
                <div style="font-size: 4rem; font-weight: bold; color: #4facfe;">1</div>
                <p style="font-size: 1.2rem;">Oferecemos soluções personalizadas para atender às suas necessidades.</p>
            </div>
            <div style="margin-bottom: 2rem;">
                <div style="font-size: 4rem; font-weight: bold; color: #4facfe;">2</div>
                <p style="font-size: 1.2rem;">Equipe altamente qualificada e experiente.</p>
            </div>
            <div style="margin-bottom: 2rem;">
                <div style="font-size: 4rem; font-weight: bold; color: #4facfe;">3</div>
                <p style="font-size: 1.2rem;">Resultados comprovados com clientes satisfeitos.</p>
            </div>
        </div>
    </section>
    
    

    <section id="services">
        <h2>Serviços</h2>
        <p>Oferecemos uma ampla gama de serviços projetados para atender às suas necessidades específicas.</p>
        <button class="cta">Saiba Mais</button>
    </section>

    <section id="video">
        <h2>Nosso Vídeo</h2>
        <p>Assista ao nosso vídeo informativo abaixo para conhecer mais sobre o que fazemos:</p>
        <video controls width="80%">
            <source src="videeo.mp4" type="video/mp4">
            Seu navegador não suporta a reprodução de vídeos.
        </video>
        <button class="cta-video" onclick="openModal()">Quero participar</button>
    </section>
    
    

    <section id="contact">
        <h2>Contato</h2>
        <p>Está pronto para trabalhar conosco? Entre em contato agora mesmo!</p>
        <button class="cta">Fale Conosco</button>
    </section>

    <footer>
        <p>&copy; 2024 Nossa Empresa. Todos os direitos reservados.</p>
    </footer>

    <div id="formModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal()">&times;</span>
            <h2>Inscreva-se</h2>
            <form>
                <div class="form-group">
                    <label for="name">Nome:</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">E-mail:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="whatsapp">WhatsApp:</label>
                    <input type="text" id="whatsapp" name="whatsapp" required>
                </div>
                <button type="submit" class="cta">Enviar</button>
            </form>
        </div>
    </div>

    <script>
        function openModal() {
            document.getElementById('formModal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('formModal').style.display = 'none';
        }
    </script>
</body>
</html>
