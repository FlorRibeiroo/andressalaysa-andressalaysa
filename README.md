<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub - Andressa Laysa</title>
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
            padding: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .github-profile {
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-bottom: 30px;
        }
        
        .profile-header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
            padding: 30px;
            position: relative;
        }
        
        .profile-content {
            padding: 30px;
        }
        
        .profile-info {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid white;
            background: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 25px;
        }
        
        .avatar i {
            font-size: 50px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .user-details h1 {
            font-size: 28px;
            margin-bottom: 5px;
        }
        
        .user-details p {
            opacity: 0.9;
            margin-bottom: 10px;
        }
        
        .badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 14px;
            margin-right: 8px;
            margin-bottom: 8px;
        }
        
        .stats {
            display: flex;
            gap: 20px;
            margin: 20px 0;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary);
        }
        
        .stat-label {
            font-size: 14px;
            color: #666;
        }
        
        .section {
            margin-bottom: 30px;
        }
        
        .section-title {
            font-size: 22px;
            color: var(--primary);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--accent);
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 20px;
        }
        
        .skill {
            background: var(--light);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 14px;
            color: var(--dark);
            border: 1px solid #ddd;
        }
        
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .project {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: var(--transition);
        }
        
        .project:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
        
        .project-header {
            background: linear-gradient(135deg, var(--accent) 0%, var(--primary) 100%);
            color: white;
            padding: 15px;
        }
        
        .project-body {
            padding: 15px;
        }
        
        .project-footer {
            padding: 15px;
            background: var(--light);
            display: flex;
            justify-content: space-between;
            font-size: 14px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: var(--primary);
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        .quote {
            font-style: italic;
            color: #666;
            border-left: 4px solid var(--accent);
            padding-left: 15px;
            margin: 20px 0;
        }
        
        @media (max-width: 768px) {
            .profile-info {
                flex-direction: column;
                text-align: center;
            }
            
            .avatar {
                margin: 0 auto 20px;
            }
            
            .stats {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .projects {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="github-profile">
        <div class="profile-header">
            <div class="profile-info">
                <div class="avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="user-details">
                    <h1>Andressa Laysa</h1>
                    <p>Desenvolvedora Front-End & Pesquisadora em Saúde e Tecnologia</p>
                    <div>
                        <span class="badge">Mestra em Eng. Biomédica</span>
                        <span class="badge">Professora</span>
                        <span class="badge">Pesquisadora</span>
                        <span class="badge">Arte-Educadora</span>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="profile-content">
            <div class="section">
                <h2 class="section-title">Sobre</h2>
                <p>Multidisciplinar por natureza, uni <strong>tecnologia, saúde e arte</strong> para criar soluções que transformam vidas e comunidades. Com mais de 10 anos de experiência em docência, pesquisa e gestão de projetos.</p>
                
                <div class="quote">
                    "Ciência, arte e política são meus instrumentos de mudança. Vamos juntos transformar realidades?"
                </div>
            </div>
            
            <div class="section">
                <h2 class="section-title">Habilidades Técnicas</h2>
                <div class="skills">
                    <span class="skill">HTML5</span>
                    <span class="skill">CSS3</span>
                    <span class="skill">JavaScript</span>
                    <span class="skill">React</span>
                    <span class="skill">Next.js</span>
                    <span class="skill">Git</span>
                    <span class="skill">Jest</span>
                    <span class="skill">Cypress</span>
                    <span class="skill">APIs REST</span>
                    <span class="skill">GraphQL</span>
                    <span class="skill">UI/UX</span>
                    <span class="skill">Responsive Design</span>
                </div>
            </div>
            
            <div class="section">
                <h2 class="section-title">Estatísticas</h2>
                <div class="stats">
                    <div class="stat">
                        <div class="stat-number">10+</div>
                        <div class="stat-label">Anos de Experiência</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">500+</div>
                        <div class="stat-label">Estudantes Ensinados</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">15+</div>
                        <div class="stat-label">Projetos Concluídos</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">5</div>
                        <div class="stat-label">Áreas de Atuação</div>
                    </div>
                </div>
            </div>
            
            <div class="section">
                <h2 class="section-title">Projetos em Destaque</h2>
                <div class="projects">
                    <div class="project">
                        <div class="project-header">
                            <h3>Plataforma de Ensino Front-End</h3>
                        </div>
                        <div class="project-body">
                            <p>Desenvolvimento de plataforma educacional para o programa Bolsa Futuro Digital.</p>
                        </div>
                        <div class="project-footer">
                            <span>React, Next.js, CSS</span>
                            <a href="#"><i class="fas fa-external-link-alt"></i></a>
                        </div>
                    </div>
                    
                    <div class="project">
                        <div class="project-header">
                            <h3>Sistema de Saúde Integrado</h3>
                        </div>
                        <div class="project-body">
                            <p>Interface para sistema de monitoramento de dados em saúde para o ICEIS-INCT.</p>
                        </div>
                        <div class="project-footer">
                            <span>JavaScript, APIs, UX/UI</span>
                            <a href="#"><i class="fas fa-external-link-alt"></i></a>
                        </div>
                    </div>
                    
                    <div class="project">
                        <div class="project-header">
                            <h3>App Dançaterapia</h3>
                        </div>
                        <div class="project-body">
                            <p>Aplicativo para acompanhamento de sessões de dançaterapia para terceira idade.</p>
                        </div>
                        <div class="project-footer">
                            <span>React Native, Node.js</span>
                            <a href="#"><i class="fas fa-external-link-alt"></i></a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="section">
                <h2 class="section-title">Contato</h2>
                <p>Disponível para palestras, cursos, consultorias e liderança de projetos que potencializem transformação social e inovação.</p>
                
                <div class="social-links">
                    <a href="#" title="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" title="GitHub"><i class="fab fa-github"></i></a>
                    <a href="#" title="E-mail"><i class="far fa-envelope"></i></a>
                    <a href="#" title="Lattes"><i class="ai ai-lattes">L</i></a>
                    <a href="#" title="Twitter"><i class="fab fa-twitter"></i></a>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Animação simples para os elementos
        document.addEventListener('DOMContentLoaded', function() {
            // Animação para os cards de projetos
            const projects = document.querySelectorAll('.project');
            projects.forEach((project, index) => {
                project.style.opacity = '0';
                project.style.transform = 'translateY(20px)';
                project.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                
                setTimeout(() => {
                    project.style.opacity = '1';
                    project.style.transform = 'translateY(0)';
                }, 200 + (index * 100));
            });
            
            // Animação para as habilidades
            const skills = document.querySelectorAll('.skill');
            skills.forEach((skill, index) => {
                skill.style.opacity = '0';
                skill.style.transform = 'scale(0.8)';
                skill.style.transition = 'opacity 0.3s ease, transform 0.3s ease';
                
                setTimeout(() => {
                    skill.style.opacity = '1';
                    skill.style.transform = 'scale(1)';
                }, 500 + (index * 50));
            });
            
            // Efeito de digitação para a citação
            const quote = document.querySelector('.quote');
            const originalText = quote.textContent;
            quote.textContent = '';
            
            let i = 0;
            function typeWriter() {
                if (i < originalText.length) {
                    quote.textContent += originalText.charAt(i);
                    i++;
                    setTimeout(typeWriter, 30);
                }
            }
            
            setTimeout(typeWriter, 1000);
        });
    </script>
</body>
</html>
