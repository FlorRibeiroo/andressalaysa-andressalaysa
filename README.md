<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Andressa Laysa | Front-End & Pesquisadora</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2D5B7A;
            --secondary: #E76F51;
            --accent: #2A9D8F;
            --light: #F8F9FA;
            --dark: #264653;
            --text: #333333;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--text);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
            padding: 2rem 0;
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        
        .profile-info {
            flex: 1;
            min-width: 300px;
        }
        
        .profile-image {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 5px solid rgba(255, 255, 255, 0.3);
            background-color: #ccc;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 2rem;
            overflow: hidden;
        }
        
        .profile-image i {
            font-size: 5rem;
            color: rgba(255, 255, 255, 0.7);
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            font-weight: 700;
        }
        
        .tagline {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: rgba(255, 255, 255, 0.9);
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.2);
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        /* About Section */
        .about {
            padding: 5rem 0;
            background: white;
        }
        
        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--primary);
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--secondary);
            margin: 0.5rem auto;
            border-radius: 2px;
        }
        
        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .about-card {
            background: var(--light);
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }
        
        .about-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
        
        .about-card i {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }
        
        .about-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--dark);
        }
        
        /* Skills Section */
        .skills {
            padding: 5rem 0;
            background: linear-gradient(to bottom, #f8f9fa, #e9ecef);
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .skill-category {
            background: white;
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .skill-category h3 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .skill-items {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
        }
        
        .skill-item {
            background: var(--light);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            color: var(--dark);
            border: 1px solid #ddd;
            transition: var(--transition);
        }
        
        .skill-item:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-2px);
        }
        
        /* Projects Section */
        .projects {
            padding: 5rem 0;
            background: white;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background: var(--light);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
        
        .project-image {
            height: 200px;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project-content h3 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        .project-content p {
            color: #666;
            margin-bottom: 1rem;
            font-size: 0.9rem;
        }
        
        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .project-tag {
            background: rgba(45, 91, 122, 0.1);
            color: var(--primary);
            padding: 0.3rem 0.7rem;
            border-radius: 15px;
            font-size: 0.8rem;
        }
        
        .project-link {
            display: inline-block;
            color: var(--secondary);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
        }
        
        .project-link:hover {
            color: var(--primary);
        }
        
        /* Contact Section */
        .contact {
            padding: 5rem 0;
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
        }
        
        .contact .section-title {
            color: white;
        }
        
        .contact-content {
            text-align: center;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .contact-content p {
            margin-bottom: 2rem;
            font-size: 1.1rem;
        }
        
        .contact-btn {
            display: inline-block;
            background: var(--secondary);
            color: white;
            padding: 1rem 2rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            font-size: 1.1rem;
        }
        
        .contact-btn:hover {
            background: white;
            color: var(--secondary);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .footer-links {
            display: flex;
            gap: 2rem;
            margin: 1.5rem 0;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            color: var(--secondary);
        }
        
        .copyright {
            margin-top: 1rem;
            color: rgba(255, 255, 255, 0.5);
            font-size: 0.9rem;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-image {
                margin: 0 auto 1.5rem;
            }
            
            h1 {
                font-size: 2.5rem;
            }
            
            .tagline {
                font-size: 1.2rem;
            }
            
            .social-links {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="profile-image">
                    <i class="fas fa-user"></i>
                </div>
                <div class="profile-info">
                    <h1>Andressa Laysa</h1>
                    <p class="tagline">Front-End Developer & Pesquisadora em Saúde e Tecnologia</p>
                    <p>Unindo ciência, arte e tecnologia para transformar vidas e comunidades</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-github"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fas fa-envelope"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- About Section -->
    <section class="about">
        <div class="container">
            <h2 class="section-title">Sobre Mim</h2>
            <div class="about-grid">
                <div class="about-card">
                    <i class="fas fa-graduation-cap"></i>
                    <h3>Formação</h3>
                    <p>Mestra em Engenharia Biomédica - UFPE</p>
                    <p>Bacharel em Enfermagem - UPE</p>
                    <p>Licencianda em Dança - UFPE</p>
                </div>
                <div class="about-card">
                    <i class="fas fa-briefcase"></i>
                    <h3>Atuação</h3>
                    <p>Professora de Front-End - Bolsa Futuro Digital</p>
                    <p>Pesquisadora - ICEIS-INCT e CEMJ Brasil</p>
                    <p>Arte-Educadora - Prefeitura do Recife</p>
                </div>
                <div class="about-card">
                    <i class="fas fa-heart"></i>
                    <h3>Propósito</h3>
                    <p>Desenvolver soluções tecnológicas que integram saúde, educação e arte para impactar positivamente a sociedade.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section class="skills">
        <div class="container">
            <h2 class="section-title">Habilidades</h2>
            <div class="skills-container">
                <div class="skill-category">
                    <h3><i class="fas fa-code"></i> Front-End</h3>
                    <div class="skill-items">
                        <span class="skill-item">HTML5</span>
                        <span class="skill-item">CSS3</span>
                        <span class="skill-item">JavaScript</span>
                        <span class="skill-item">React</span>
                        <span class="skill-item">Next.js</span>
                        <span class="skill-item">Responsive Design</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3><i class="fas fa-cogs"></i> Ferramentas</h3>
                    <div class="skill-items">
                        <span class="skill-item">Git</span>
                        <span class="skill-item">GitHub</span>
                        <span class="skill-item">Jest</span>
                        <span class="skill-item">Cypress</span>
                        <span class="skill-item">Figma</span>
                        <span class="skill-item">VS Code</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3><i class="fas fa-flask"></i> Pesquisa</h3>
                    <div class="skill-items">
                        <span class="skill-item">Metodologia Científica</span>
                        <span class="skill-item">ABNT/APA</span>
                        <span class="skill-item">Análise de Dados</span>
                        <span class="skill-item">Escrita Acadêmica</span>
                        <span class="skill-item">Gestão de Projetos</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="projects">
        <div class="container">
            <h2 class="section-title">Projetos em Destaque</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <div class="project-content">
                        <h3>Plataforma de Ensino Front-End</h3>
                        <p>Desenvolvimento de plataforma educacional para o programa Bolsa Futuro Digital.</p>
                        <div class="project-tags">
                            <span class="project-tag">React</span>
                            <span class="project-tag">Next.js</span>
                            <span class="project-tag">CSS3</span>
                        </div>
                        <a href="#" class="project-link">Ver Projeto <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-heartbeat"></i>
                    </div>
                    <div class="project-content">
                        <h3>Sistema de Saúde Integrado</h3>
                        <p>Interface para sistema de monitoramento de dados em saúde para o ICEIS-INCT.</p>
                        <div class="project-tags">
                            <span class="project-tag">JavaScript</span>
                            <span class="project-tag">APIs</span>
                            <span class="project-tag">UX/UI</span>
                        </div>
                        <a href="#" class="project-link">Ver Projeto <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-dragon"></i>
                    </div>
                    <div class="project-content">
                        <h3>App Dançaterapia</h3>
                        <p>Aplicativo para acompanhamento de sessões de dançaterapia para terceira idade.</p>
                        <div class="project-tags">
                            <span class="project-tag">React Native</span>
                            <span class="project-tag">Node.js</span>
                            <span class="project-tag">MongoDB</span>
                        </div>
                        <a href="#" class="project-link">Ver Projeto <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact">
        <div class="container">
            <h2 class="section-title">Vamos Conversar?</h2>
            <div class="contact-content">
                <p>Estou disponível para palestras, cursos, consultorias e liderança de projetos que potencializem transformação social, inovação e resultados.</p>
                <a href="mailto:andressa.laysa@ufpe.br" class="contact-btn">Entrar em Contato</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <h3>Andressa Laysa</h3>
                <div class="footer-links">
                    <a href="#">LinkedIn</a>
                    <a href="#">Lattes</a>
                    <a href="#">GitHub</a>
                    <a href="#">Instagram</a>
                </div>
                <p class="copyright">© 2023 Andressa Laysa. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple animation for skills on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const skillItems = document.querySelectorAll('.skill-item');
            
            skillItems.forEach((item, index) => {
                // Add delay for staggered animation
                item.style.animationDelay = `${index * 0.1}s`;
            });
            
            // Add hover effect to project cards
            const projectCards = document.querySelectorAll('.project-card');
            projectCards.forEach(card => {
                card.addEventListener('mouseenter', () => {
                    card.querySelector('.project-link').style.color = '#E76F51';
                });
                
                card.addEventListener('mouseleave', () => {
                    card.querySelector('.project-link').style.color = '#2D5B7A';
                });
            });
        });
    </script>
</body>
</html>
