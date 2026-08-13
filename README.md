<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mon Portfolio - Réseaux & Télécommunications</title>
    <style>
        :root {
            --primary-color: #0f172a;
            --secondary-color: #3b82f6;
            --accent-color: #10b981;
            --bg-color: #f8fafc;
            --card-bg: #ffffff;
            --text-color: #334155;
            --text-light: #64748b;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), #1e293b);
            color: white;
            padding: 4rem 2rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
            color: #ffffff;
        }

        header p {
            font-size: 1.2rem;
            color: #94a3b8;
            max-width: 600px;
            margin: 0 auto;
        }

        nav {
            background-color: white;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
            display: flex;
            justify-content: center;
            gap: 2rem;
            padding: 1rem;
        }

        nav a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 600;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 3rem 2rem;
        }

        section {
            margin-bottom: 4rem;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            color: var(--primary-color);
            border-bottom: 3px solid var(--secondary-color);
            display: inline-block;
            padding-bottom: 0.3rem;
        }

        .about-content {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            font-size: 1.1rem;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .skill-card {
            background: var(--card-bg);
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            border-left: 4px solid var(--secondary-color);
        }

        .skill-card h3 {
            margin-bottom: 0.8rem;
            color: var(--primary-color);
        }

        .skill-card ul {
            list-style-type: none;
        }

        .skill-card li {
            margin-bottom: 0.4rem;
            color: var(--text-light);
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: var(--card-bg);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
            display: flex;
            flex-direction: column;
        }

        .project-card:hover {
            transform: translateY(-5px);
        }

        .project-header {
            background-color: var(--primary-color);
            color: white;
            padding: 1.2rem;
        }

        .project-body {
            padding: 1.5rem;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .project-body p {
            color: var(--text-light);
            margin-bottom: 1rem;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1.2rem;
        }

        .tag {
            background-color: #e2e8f0;
            color: var(--primary-color);
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        .btn {
            display: inline-block;
            background-color: var(--secondary-color);
            color: white;
            padding: 0.6rem 1.2rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: 600;
            text-align: center;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #2563eb;
        }

        footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        footer p {
            color: #94a3b8;
        }
    </style>
</head>
<body>

    <header>
        <h1>Nom Prénom</h1>
        <p>Étudiante en Réseaux & Télécommunications | Passionnée par l'infrastructure réseau, la cybersécurité et l'administration système</p>
    </header>

    <nav>
        <a href="#about">À propos</a>
        <a href="#skills">Compétences</a>
        <a href="#projects">Projets & TPs</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">
        
        <!-- Section À propos -->
        <section id="about">
            <h2>À propos de moi</h2>
            <div class="about-content">
                <p>Actuellement étudiante en filière Réseaux et Télécommunications, je me passionne pour la conception, la sécurisation et l'optimisation des architectures réseaux et des systèmes informatiques. Curieuse et rigoureuse, j'aime mettre en pratique mes connaissances à travers des TPs techniques, des configurations de routeurs/switches et le déploiement de services sous Linux.</p>
            </div>
        </section>

        <!-- Section Compétences -->
        <section id="skills">
            <h2>Compétences Techniques</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <h3>Réseaux</h3>
                    <ul>
                        <li>Routage & Commutation (VLAN, STP, OSPF, EIGRP)</li>
                        <li>Modèle OSI & TCP/IP, Analyse de trames (Wireshark)</li>
                        <li>Simulation : Cisco Packet Tracer, GNS3, eNSP</li>
                    </ul>
                </div>
                <div class="skill-card">
                    <h3>Systèmes & Sécurité</h3>
                    <ul>
                        <li>Administration Linux (Bash, Permissions, SSH)</li>
                        <li>Services Réseau (DNS, DHCP, Apache, FTP)</li>
                        <li>Sécurité de base (Firewalls, VPN, Metasploitable)</li>
                    </ul>
                </div>
                <div class="skill-card">
                    <h3>Télécoms & Outils</h3>
                    <ul>
                        <li>Supports de transmission & Téléphonie IP (VoIP)</li>
                        <li>Gestion de projets (PERT, Gantt)</li>
                        <li>Contrôle de version : Git / GitHub</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Section Projets & TPs -->
        <section id="projects">
            <h2>Mes Projets & TPs Réalisés</h2>
            <div class="projects-grid">
                
                <!-- Projet 1 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Architecture Réseau d'Entreprise</h3>
                    </div>
                    <div class="project-body">
                        <p>Conception et simulation d'un réseau multi-sites sécurisé avec segmentation VLAN, mise en place du protocole OSPF et configuration des listes de contrôle d'accès (ACL).</p>
                        <div class="tags">
                            <span class="tag">Cisco Packet Tracer</span>
                            <span class="tag">OSPF</span>
                            <span class="tag">VLAN</span>
                        </div>
                        <a href="#" class="btn">Voir les détails</a>
                    </div>
                </div>

                <!-- Projet 2 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Déploiement de Serveurs Linux</h3>
                    </div>
                    <div class="project-body">
                        <p>Installation et configuration complète d'un serveur sous Linux (Ubuntu/Debian) intégrant un serveur DHCP, un serveur DNS (BIND9) et un serveur Web sécurisé (HTTPS).</p>
                        <div class="tags">
                            <span class="tag">Linux</span>
                            <span class="tag">DNS/DHCP</span>
                            <span class="tag">Bash</span>
                        </div>
                        <a href="#" class="btn">Voir les détails</a>
                    </div>
                </div>

                <!-- Projet 3 -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Analyse de Trafic & Sécurité</h3>
                    </div>
                    <div class="project-body">
                        <p>TP pratique d'analyse de trames réseau suspectes avec Wireshark et exploitation contrôlée d'une machine virtuelle vulnérable (Metasploitable) dans un lab isolé.</p>
                        <div class="tags">
                            <span class="tag">Wireshark</span>
                            <span class="tag">Cybersécurité</span>
                            <span class="tag">Metasploitable</span>
                        </div>
                        <a href="#" class="btn">Voir les détails</a>
                    </div>
                </div>

            </div>
        </section>

        <!-- Section Contact -->
        <section id="contact">
            <h2>Contact</h2>
            <div class="about-content" style="text-align: center;">
                <p>Je suis actuellement à la recherche d'un stage dans le domaine des réseaux et télécommunications.</p>
                <p style="margin-top: 1rem;">
                    <strong>Email :</strong> votre.email@etudiant.univ.fr<br>
                    <strong>LinkedIn :</strong> linkedin.com/in/votre-nom<br>
                    <strong>GitHub :</strong> github.com/votre-compte
                </p>
            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 - Portfolio | Étudiante en Réseaux & Télécommunications</p>
    </footer>

</body>
</html>
