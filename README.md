<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KANABE PEUDEBYA ALBERT - Analyste Statisticien</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f4f4f4;
        }

        /* Navigation */
        nav {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav .container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }

        nav h1 {
            font-size: 1.5rem;
            font-weight: 700;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
            padding: 5px 10px;
            border-radius: 5px;
        }

        nav a:hover {
            background: rgba(255,255,255,0.2);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 150px 20px 100px;
            text-align: center;
            margin-top: 60px;
        }

        .profile-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }

        .profile-photo {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 6px solid white;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            overflow: hidden;
            background: white;
        }

        .profile-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 10px;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        .hero .subtitle {
            font-size: 1.3rem;
            opacity: 0.95;
            margin-bottom: 10px;
        }

        .hero .location {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Sections */
        section {
            padding: 60px 20px;
            background: white;
            margin: 20px auto;
            max-width: 1200px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        section h2 {
            color: #667eea;
            font-size: 2.2rem;
            margin-bottom: 40px;
            text-align: center;
            position: relative;
            padding-bottom: 15px;
        }

        section h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 2px;
        }

        /* About */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin-top: 30px;
        }

        .info-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 10px;
            border-left: 5px solid #667eea;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .info-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
        }

        .info-card h3 {
            color: #667eea;
            margin-bottom: 15px;
            font-size: 1.4rem;
        }

        .info-card p, .info-card ul {
            color: #555;
            line-height: 1.8;
        }

        .info-card ul {
            list-style-position: inside;
            margin-left: 10px;
        }

        /* Skills */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .skill-card {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .skill-card:hover {
            transform: translateY(-10px);
        }

        .skill-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .skill-card p {
            opacity: 0.95;
            line-height: 1.6;
        }

        /* Projects */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .project-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            border: 2px solid #f0f0f0;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .project-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
        }

        .project-content {
            padding: 25px;
        }

        .project-content h3 {
            color: #667eea;
            margin-bottom: 15px;
            font-size: 1.4rem;
        }

        .project-content p {
            color: #666;
            margin-bottom: 15px;
            line-height: 1.8;
        }

        .project-tags {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        .tag {
            background: #e3f2fd;
            color: #1976d2;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        /* CV Section */
        .cv-section {
            text-align: center;
            padding: 60px 20px;
        }

        .cv-download {
            display: inline-flex;
            align-items: center;
            gap: 15px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: 600;
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
            transition: all 0.3s;
            margin-top: 20px;
        }

        .cv-download:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.6);
        }

        .cv-icon {
            font-size: 2rem;
        }

        /* Contact */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .contact-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s;
        }

        .contact-card:hover {
            transform: translateY(-5px);
        }

        .contact-icon {
            font-size: 3rem;
            margin-bottom: 15px;
        }

        .contact-card h3 {
            color: #667eea;
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .contact-card a {
            color: #555;
            text-decoration: none;
            font-weight: 500;
            word-break: break-word;
        }

        .contact-card a:hover {
            color: #667eea;
        }

        /* Footer */
        footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 30px 20px;
            margin-top: 40px;
        }

        footer p {
            opacity: 0.9;
        }

        /* Responsive */
        @media (max-width: 768px) {
            nav ul {
                gap: 1rem;
                font-size: 0.9rem;
            }

            nav h1 {
                font-size: 1.2rem;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .profile-photo {
                width: 150px;
                height: 150px;
            }
        }

        /* Smooth scroll */
        html {
            scroll-behavior: smooth;
        }

        /* Modal for enlarged photo */
        .modal {
            display: none;
            position: fixed;
            z-index: 9999;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.9);
            animation: fadeIn 0.3s;
        }

        .modal-content {
            position: relative;
            margin: auto;
            display: block;
            max-width: 90%;
            max-height: 90%;
            top: 50%;
            transform: translateY(-50%);
            animation: zoomIn 0.3s;
        }

        .close-modal {
            position: absolute;
            top: 30px;
            right: 50px;
            color: white;
            font-size: 50px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
        }

        .close-modal:hover {
            color: #667eea;
        }

        @keyframes fadeIn {
            from {opacity: 0;}
            to {opacity: 1;}
        }

        @keyframes zoomIn {
            from {transform: translateY(-50%) scale(0.8);}
            to {transform: translateY(-50%) scale(1);}
        }

        .profile-photo {
            cursor: pointer;
        }

        .modal-caption {
            text-align: center;
            color: white;
            padding: 20px;
            font-size: 1.3rem;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="container">
            <h1>KANABE PEUDEBYA ALBERT</h1>
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#apropos">À propos</a></li>
                <li><a href="#competences">Compétences</a></li>
                <li><a href="#projets">Projets</a></li>
                <li><a href="#cv">CV</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="accueil" class="hero">
        <div class="profile-container">
            <div class="profile-photo">
                <img src="profile.jpeg" alt="KANABE PEUDEBYA ALBERT">
            </div>
            <h2>KANABE PEUDEBYA ALBERT</h2>
            <p class="subtitle">Étudiant en Analyse Statistique (AS2)</p>
            <p class="location">📍 ENSEA - Abidjan, Côte d'Ivoire</p>
        </div>
    </section>

    <!-- About Section -->
    <section id="apropos">
        <h2>À propos de moi</h2>
        <div class="about-content">
            <div class="info-card">
                <h3>🎓 Formation Actuelle</h3>
                <p><strong>École Nationale Supérieure de Statistique et d'Économie Appliquée (ENSEA)</strong></p>
                <p>Deuxième année d'Analyse Statistique (AS2)</p>
                <p>Abidjan, Côte d'Ivoire</p>
                <p style="margin-top: 10px;"><em>Prochainement : AS3 - Spécialisation Data Science</em></p>
            </div>
            <div class="info-card">
                <h3>🎯 Objectifs et Ambitions</h3>
                <p>Étudiant motivé en statistique, je me prépare à me spécialiser en Data Science dès ma troisième année. Passionné par l'analyse de données, j'aspire à développer mes compétences en intelligence artificielle et en analyse avancée.</p>
            </div>
            <div class="info-card">
                <h3>💡 Centres d'intérêt</h3>
                <ul>
                    <li>Data Science et Big Data</li>
                    <li>Intelligence Artificielle et Machine Learning</li>
                    <li>Analyse prédictive</li>
                    <li>Programmation statistique</li>
                    <li>Visualisation de données</li>
                </ul>
            </div>
            <div class="info-card">
                <h3>🌍 Langues</h3>
                <ul>
                    <li>Français - Langue maternelle</li>
                    <li>Anglais - Niveau intermédiaire</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="competences">
        <h2>Mes Compétences</h2>
        <div class="skills-grid">
            <div class="skill-card">
                <h3>📊 Analyse Statistique</h3>
                <p>Formation en cours : statistiques descriptives, probabilités, tests statistiques. En apprentissage continu pour maîtriser l'analyse de données complexes.</p>
            </div>
            <div class="skill-card">
                <h3>💻 Programmation</h3>
                <p>Initiation à R, Python, et Excel. En cours d'acquisition des compétences en programmation statistique pour la Data Science.</p>
            </div>
            <div class="skill-card">
                <h3>🎓 Formation Continue</h3>
                <p>Actuellement en AS2, je consolide mes bases en statistiques et mathématiques appliquées en préparation de ma spécialisation en Data Science.</p>
            </div>
            <div class="skill-card">
                <h3>🚀 Prochaines Étapes</h3>
                <p>À partir de l'année prochaine (AS3) : Machine Learning, Deep Learning, Big Data Analytics, et projets Data Science avancés.</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projets">
        <h2>Mes Projets</h2>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-image">📊</div>
                <div class="project-content">
                    <h3>Projets Académiques AS2</h3>
                    <p>Travaux pratiques et études de cas en analyse statistique dans le cadre de ma formation à l'ENSEA. Projets à venir et en développement.</p>
                    <div class="project-tags">
                        <span class="tag">Statistiques</span>
                        <span class="tag">R</span>
                        <span class="tag">Analyse de données</span>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-image">🎯</div>
                <div class="project-content">
                    <h3>Futurs Projets Data Science</h3>
                    <p>Espace réservé pour mes futurs projets en Data Science à partir de l'année prochaine : Machine Learning, prédiction, analyse prédictive.</p>
                    <div class="project-tags">
                        <span class="tag">Python</span>
                        <span class="tag">Machine Learning</span>
                        <span class="tag">Data Science</span>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-image">💡</div>
                <div class="project-content">
                    <h3>Projets Personnels</h3>
                    <p>Espace dédié à mes projets personnels et auto-apprentissage en programmation et analyse de données. En construction continue.</p>
                    <div class="project-tags">
                        <span class="tag">Apprentissage</span>
                        <span class="tag">Innovation</span>
                        <span class="tag">Portfolio</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CV Section -->
    <section id="cv" class="cv-section">
        <h2>Mon Curriculum Vitae</h2>
        <p style="color: #666; font-size: 1.1rem; margin-bottom: 20px;">
            Téléchargez mon CV complet pour découvrir mon parcours détaillé, mes expériences et mes réalisations académiques.
        </p>
        <a href="CV_KANABE_PEUDEBYA_ALBERT.pdf" class="cv-download" download>
            <span class="cv-icon">📄</span>
            <span>Télécharger mon CV</span>
        </a>
        <p style="color: #999; font-size: 0.9rem; margin-top: 20px;">
            Format PDF • Dernière mise à jour : Février 2026
        </p>
        <p style="color: #ff6b6b; font-size: 0.95rem; margin-top: 15px; font-style: italic;">
            Note : Veuillez uploader votre CV en PDF avec le nom "CV_KANABE_PEUDEBYA_ALBERT.pdf" dans votre repository GitHub pour activer le téléchargement.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Me Contacter</h2>
        <div class="contact-grid">
            <div class="contact-card">
                <div class="contact-icon">📧</div>
                <h3>Email</h3>
                <a href="mailto:albertkanabepeudebya@gmail.com">albertkanabepeudebya@gmail.com</a>
            </div>
            <div class="contact-card">
                <div class="contact-icon">💼</div>
                <h3>LinkedIn</h3>
                <a href="https://www.linkedin.com/in/albert-kanabe-peudebya" target="_blank">Albert Kanabe Peudebya</a>
            </div>
            <div class="contact-card">
                <div class="contact-icon">💻</div>
                <h3>GitHub</h3>
                <a href="https://github.com/KANABE-PEUDEBYA-ALBERT" target="_blank">KANABE-PEUDEBYA-ALBERT</a>
            </div>
            <div class="contact-card">
                <div class="contact-icon">📱</div>
                <h3>Téléphone</h3>
                <a href="tel:+22501419627339">+225 01 41 96 27 39</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 KANABE PEUDEBYA ALBERT. Tous droits réservés.</p>
        <p style="margin-top: 10px; opacity: 0.8;">Étudiant en Analyse Statistique - ENSEA Abidjan</p>
        <p style="margin-top: 5px; opacity: 0.7; font-size: 0.9rem;">Futur Data Scientist 🚀</p>
    </footer>

    <!-- Modal for enlarged photo -->
    <div id="photoModal" class="modal">
        <span class="close-modal" onclick="closeModal()">&times;</span>
        <img class="modal-content" id="modalImage">
        <div class="modal-caption">KANABE PEUDEBYA ALBERT - Étudiant en Analyse Statistique</div>
    </div>

    <script>
        // Open modal when profile photo is clicked
        document.querySelector('.profile-photo img').addEventListener('click', function() {
            var modal = document.getElementById('photoModal');
            var modalImg = document.getElementById('modalImage');
            modal.style.display = 'block';
            modalImg.src = this.src;
        });

        // Close modal function
        function closeModal() {
            document.getElementById('photoModal').style.display = 'none';
        }

        // Close modal when clicking outside the image
        document.getElementById('photoModal').addEventListener('click', function(event) {
            if (event.target === this) {
                closeModal();
            }
        });

        // Close modal with Escape key
        document.addEventListener('keydown', function(event) {
            if (event.key === 'Escape') {
                closeModal();
            }
        });
    </script>
</body>
</html>
