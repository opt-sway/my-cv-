<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Azer Rached - CV Créatif</title>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Bebas+Neue&family=Bangers&family=Roboto:wght@300;400;700;900&family=Permanent+Marker&display=swap" rel="stylesheet">
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  font-family: 'Roboto', sans-serif;
  background: #f0f0f0;
  overflow-x: hidden;
}

.cv-container {
  max-width: 1200px;
  margin: 0 auto;
  background: white;
  position: relative;
  padding: 30px;
}

/* Comic Book Style Burst */
.burst {
  position: absolute;
  font-family: 'Bangers', cursive;
  z-index: 10;
}

.burst-1 {
  top: 40px;
  right: 80px;
  background: #FF6B35;
  color: white;
  padding: 15px 25px;
  font-size: 24px;
  transform: rotate(12deg);
  border: 4px solid #000;
  box-shadow: 5px 5px 0 rgba(0,0,0,0.3);
}

.burst-2 {
  top: 150px;
  left: 50px;
  background: #FFD700;
  color: #000;
  padding: 12px 20px;
  font-size: 18px;
  transform: rotate(-8deg);
  border: 4px solid #000;
  box-shadow: 5px 5px 0 rgba(0,0,0,0.3);
}

.burst-3 {
  bottom: 200px;
  right: 60px;
  background: #4ECDC4;
  color: #000;
  padding: 15px 25px;
  font-size: 20px;
  transform: rotate(15deg);
  border: 4px solid #000;
  box-shadow: 5px 5px 0 rgba(0,0,0,0.3);
}

/* Main Grid Layout */
.main-grid {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 30px;
  margin-top: 20px;
}

/* Header Section */
.header {
  grid-column: 1 / -1;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  padding: 40px;
  border: 8px solid #000;
  position: relative;
  overflow: hidden;
}

.header::before {
  content: 'BAM!';
  position: absolute;
  top: -20px;
  right: 40px;
  font-family: 'Bangers', cursive;
  font-size: 120px;
  color: rgba(255,255,255,0.1);
  transform: rotate(-15deg);
}

.header-content {
  position: relative;
  z-index: 2;
}

.name-title h1 {
  font-family: 'Anton', sans-serif;
  font-size: 72px;
  color: white;
  line-height: 0.9;
  text-transform: uppercase;
  letter-spacing: -2px;
  text-shadow: 4px 4px 0 rgba(0,0,0,0.3);
}

.subtitle {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 24px;
  color: #FFD700;
  margin-top: 10px;
  letter-spacing: 2px;
}

.mission-badge {
  background: #FF6B35;
  color: white;
  padding: 15px 25px;
  display: inline-block;
  margin-top: 15px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 20px;
  border: 4px solid #000;
  box-shadow: 5px 5px 0 rgba(0,0,0,0.5);
  letter-spacing: 1px;
}

.header-stats {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 15px;
  margin-top: 25px;
}

.stat-box {
  background: #000;
  color: #FFD700;
  padding: 20px;
  text-align: center;
  border: 4px solid #FFD700;
}

.stat-box .number {
  font-family: 'Bangers', cursive;
  font-size: 36px;
  display: block;
}

.stat-box .label {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 14px;
  margin-top: 5px;
  letter-spacing: 1px;
}

/* Left Sidebar */
.sidebar {
  background: #1a1a1a;
  padding: 30px 20px;
  border: 6px solid #000;
  color: white;
}

.section-header {
  font-family: 'Bangers', cursive;
  font-size: 28px;
  color: #FFD700;
  margin: 25px 0 15px 0;
  border-bottom: 3px solid #FF6B35;
  padding-bottom: 8px;
}

.contact-item {
  margin: 15px 0;
  font-size: 14px;
  line-height: 1.8;
}

.contact-item strong {
  color: #4ECDC4;
  display: block;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 16px;
  letter-spacing: 1px;
}

.alert-box {
  background: #FF6B35;
  color: white;
  padding: 20px;
  text-align: center;
  margin: 20px 0;
  border: 4px solid #000;
  box-shadow: 5px 5px 0 rgba(255,215,0,0.5);
}

.alert-box h3 {
  font-family: 'Bangers', cursive;
  font-size: 24px;
  margin-bottom: 10px;
}

.skills-list {
  list-style: none;
  margin: 10px 0;
}

.skills-list li {
  background: linear-gradient(90deg, #4ECDC4, transparent);
  padding: 8px 12px;
  margin: 8px 0;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 16px;
  letter-spacing: 1px;
  border-left: 4px solid #FFD700;
}

.tools-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
  margin: 15px 0;
}

.tool-badge {
  background: #FFD700;
  color: #000;
  padding: 10px;
  text-align: center;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 14px;
  border: 3px solid #000;
  font-weight: bold;
}

.language-item {
  display: flex;
  justify-content: space-between;
  padding: 10px;
  margin: 8px 0;
  background: rgba(255,215,0,0.1);
  border-left: 3px solid #FFD700;
}

.language-level {
  font-family: 'Bebas Neue', sans-serif;
  color: #4ECDC4;
  font-size: 14px;
}

/* Main Content */
.main-content {
  padding: 20px;
}

.content-section {
  margin: 30px 0;
}

.content-section h2 {
  font-family: 'Bangers', cursive;
  font-size: 36px;
  color: #000;
  margin-bottom: 20px;
  position: relative;
  display: inline-block;
}

.content-section h2::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 100%;
  height: 6px;
  background: linear-gradient(90deg, #FF6B35, #FFD700);
}

.mission-box {
  background: linear-gradient(135deg, #FFD700, #FFA500);
  padding: 30px;
  border: 6px solid #000;
  box-shadow: 10px 10px 0 rgba(0,0,0,0.2);
  margin: 20px 0;
}

.mission-box h3 {
  font-family: 'Bangers', cursive;
  font-size: 28px;
  margin-bottom: 15px;
}

.mission-box p {
  font-size: 16px;
  line-height: 1.8;
  font-weight: 500;
}

.experience-card {
  background: white;
  border: 5px solid #000;
  padding: 25px;
  margin: 20px 0;
  position: relative;
  box-shadow: 8px 8px 0 rgba(0,0,0,0.1);
}

.experience-card::before {
  content: 'POW!';
  position: absolute;
  top: -15px;
  right: 20px;
  font-family: 'Bangers', cursive;
  font-size: 32px;
  background: #FF6B35;
  color: white;
  padding: 5px 20px;
  border: 3px solid #000;
  transform: rotate(8deg);
}

.experience-card:nth-child(even)::before {
  content: 'BOOM!';
  background: #4ECDC4;
  color: #000;
}

.experience-card h3 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 28px;
  color: #667eea;
  margin-bottom: 5px;
  letter-spacing: 1px;
}

.experience-card .role {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 20px;
  color: #FF6B35;
  margin-bottom: 8px;
}

.experience-card .period {
  font-size: 14px;
  color: #666;
  margin-bottom: 15px;
  font-style: italic;
}

.experience-card ul {
  margin-left: 20px;
  line-height: 1.9;
}

.experience-card ul li {
  margin: 8px 0;
}

.results-highlight {
  background: #FFD700;
  padding: 15px;
  margin: 15px 0;
  border-left: 6px solid #FF6B35;
  font-weight: bold;
}

.formation-item {
  background: linear-gradient(135deg, rgba(102,126,234,0.1), rgba(118,75,162,0.1));
  padding: 20px;
  margin: 15px 0;
  border-left: 6px solid #667eea;
}

.formation-item h4 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 22px;
  color: #667eea;
  margin-bottom: 5px;
}

.formation-item .org {
  font-size: 14px;
  color: #666;
  font-style: italic;
}

/* CTA Section */
.cta-section {
  background: #000;
  color: white;
  padding: 40px;
  text-align: center;
  border: 8px solid #FFD700;
  margin: 40px 0;
  position: relative;
}

.cta-section::before {
  content: '⚡';
  position: absolute;
  top: 20px;
  left: 30px;
  font-size: 60px;
  color: #FFD700;
}

.cta-section::after {
  content: '⚡';
  position: absolute;
  bottom: 20px;
  right: 30px;
  font-size: 60px;
  color: #FFD700;
}

.cta-section h2 {
  font-family: 'Bangers', cursive;
  font-size: 48px;
  color: #FFD700;
  margin-bottom: 20px;
}

.cta-buttons {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 25px;
}

.cta-btn {
  background: #FF6B35;
  color: white;
  padding: 20px 40px;
  text-decoration: none;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 24px;
  border: 5px solid white;
  display: inline-block;
  transition: all 0.3s;
  letter-spacing: 2px;
  box-shadow: 5px 5px 0 rgba(255,215,0,0.5);
}

.cta-btn:hover {
  transform: scale(1.05) rotate(-2deg);
  background: #FFD700;
  color: #000;
}

.social-links {
  margin-top: 20px;
  font-size: 14px;
}

.social-links a {
  color: #4ECDC4;
  text-decoration: none;
  margin: 0 10px;
}

/* Competences Grid */
.competences-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15px;
  margin: 20px 0;
}

.competence-category {
  background: white;
  border: 4px solid #000;
  padding: 20px;
  box-shadow: 6px 6px 0 rgba(0,0,0,0.1);
}

.competence-category h4 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 20px;
  color: #FF6B35;
  margin-bottom: 10px;
  border-bottom: 2px solid #FFD700;
  padding-bottom: 5px;
}

.competence-category ul {
  list-style: none;
  font-size: 14px;
  line-height: 1.8;
}

.competence-category ul li::before {
  content: '✓';
  color: #4ECDC4;
  font-weight: bold;
  margin-right: 8px;
}

/* Responsive */
@media (max-width: 968px) {
  .main-grid {
    grid-template-columns: 1fr;
  }
  
  .header-stats {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .name-title h1 {
    font-size: 48px;
  }
  
  .competences-grid {
    grid-template-columns: 1fr;
  }
}

@media print {
  .burst { display: none; }
  body { background: white; }
}
</style>
</head>
<body>

<div class="cv-container">
  
  <!-- Comic Bursts -->
  <div class="burst burst-1">8+ ANS EXP</div>
  <div class="burst burst-2">BAM!</div>
  <div class="burst burst-3">ROI PROUVÉ</div>

  <!-- Header -->
  <div class="header">
    <div class="header-content">
      <div class="name-title">
        <h1>AZER<br>RACHED</h1>
        <div class="subtitle">Marketing Digital • Entrepreneur • Stratège Commercial</div>
      </div>
      
      <div class="mission-badge">
        🎯 RECHERCHE ALTERNANCE - Assistant Commercial / Marketing Digital
      </div>

      <div class="header-stats">
        <div class="stat-box">
          <span class="number">30K+</span>
          <span class="label">Abonnés</span>
        </div>
        <div class="stat-box">
          <span class="number">20M+</span>
          <span class="label">Vues</span>
        </div>
        <div class="stat-box">
          <span class="number">50K€</span>
          <span class="label">CA/Trimestre</span>
        </div>
        <div class="stat-box">
          <span class="number">8+</span>
          <span class="label">Années Exp</span>
        </div>
      </div>
    </div>
  </div>

  <!-- Main Grid -->
  <div class="main-grid">
    
    <!-- Sidebar -->
    <div class="sidebar">
      
      <div class="alert-box">
        <h3>⚡ ALERTE RECRUTEUR!</h3>
        <p style="font-family: 'Bebas Neue', sans-serif; font-size: 18px; margin-top: 10px;">CANDIDAT DISPONIBLE</p>
        <p style="font-size: 14px; margin-top: 5px;">ALTERNANCE IMMÉDIATE</p>
      </div>

      <div class="section-header">Contact</div>
      <div class="contact-item">
        <strong>📍 Localisation</strong>
        Paris & Île-de-France
      </div>
      <div class="contact-item">
        <strong>📱 Téléphone</strong>
        <a href="tel:+33602560229" style="color: #4ECDC4; text-decoration: none;">+33 6 02 56 02 29</a>
      </div>
      <div class="contact-item">
        <strong>✉️ Email</strong>
        <a href="mailto:azerrached3@gmail.com" style="color: #4ECDC4; text-decoration: none;">azerrached3@gmail.com</a>
      </div>
      <div class="contact-item">
        <strong>🎂 Âge</strong>
        26 ans
      </div>

      <div class="section-header">Super-Pouvoirs</div>
      <ul class="skills-list">
        <li>💰 Génération de Leads</li>
        <li>🎨 Création de Contenu</li>
        <li>📊 Analyse & Stratégie</li>
        <li>🤝 Closing & Négociation</li>
        <li>👥 Leadership d'Équipe</li>
      </ul>

      <div class="section-header">Arsenal Digital</div>
      <div class="tools-grid">
        <div class="tool-badge">META ADS</div>
        <div class="tool-badge">GOOGLE ANALYTICS</div>
        <div class="tool-badge">CANVA PRO</div>
        <div class="tool-badge">CHATGPT</div>
        <div class="tool-badge">NOTION</div>
        <div class="tool-badge">CRM</div>
        <div class="tool-badge">TRELLO</div>
        <div class="tool-badge">SEO/SEM</div>
      </div>

      <div class="section-header">Langues</div>
      <div class="language-item">
        <span>🇹🇳 Arabe</span>
        <span class="language-level">NATIF</span>
      </div>
      <div class="language-item">
        <span>🇫🇷 Français</span>
        <span class="language-level">COURANT</span>
      </div>
      <div class="language-item">
        <span>🇬🇧 Anglais</span>
        <span class="language-level">COURANT</span>
      </div>
      <div class="language-item">
        <span>🇷🇺 Russe</span>
        <span class="language-level">COURANT</span>
      </div>
      <div class="language-item">
        <span>🇩🇪 Allemand</span>
        <span class="language-level">NOTIONS</span>
      </div>
      <div class="language-item">
        <span>🇪🇸 Espagnol</span>
        <span class="language-level">NOTIONS</span>
      </div>
      <div class="language-item">
        <span>🇮🇹 Italien</span>
        <span class="language-level">NOTIONS</span>
      </div>

      <div class="section-header">Passions</div>
      <div style="font-size: 14px; line-height: 2;">
        🥊 MMA & Combat Sports<br>
        🎬 Content Creation<br>
        🛒 E-Commerce<br>
        📈 Growth Hacking<br>
        💰 Crypto & Trading
      </div>

    </div>

    <!-- Main Content -->
    <div class="main-content">
      
      <!-- Mission -->
      <div class="mission-box">
        <h3>🎯 MA MISSION</h3>
        <p>Transformer les données en croissance, les idées en résultats. Entrepreneur et marketeur orienté ROI, je recherche une alternance où je peux déployer mes compétences en prospection digitale, création de contenu viral, et stratégie commerciale data-driven. Mon superpouvoir : créer des systèmes qui génèrent des revenus récurrents.</p>
      </div>

      <!-- Experience -->
      <div class="content-section">
        <h2>💼 Expérience & Résultats</h2>

        <div class="experience-card">
          <h3>Entrepreneur Indépendant</h3>
          <div class="role">Marketing Digital & Trading</div>
          <div class="period">2024 – Présent</div>
          <ul>
            <li>Construction d'une audience de 30K+ abonnés et 20M+ vues</li>
            <li>Monétisation multi-canal : dropshipping, affiliation, sponsorships</li>
            <li>Stratégies data-driven pour croissance organique et engagement</li>
          </ul>
          <div class="results-highlight">
            📈 Revenus récurrents ⚡ 20M+ vues 👥 30K communauté
          </div>
        </div>

        <div class="experience-card">
          <h3>RealSmile</h3>
          <div class="role">Chef de Projet Digital – Plateforme Médicale</div>
          <div class="period">2023 – 2024</div>
          <ul>
            <li>Pilotage du site web et app mobile RealSmile Paris</li>
            <li>Parcours patient 100% digitalisé (UX optimisée)</li>
            <li>Coordination équipes tech, design & marketing</li>
          </ul>
          <div class="results-highlight">
            🚀 -10 jours livraison 💰 -7% coûts
          </div>
        </div>

        <div class="experience-card">
          <h3>RTS Voyages</h3>
          <div class="role">Fondateur & Gérant</div>
          <div class="period">2021 – 2023</div>
          <ul>
            <li>Création et gestion agence séjours touristiques premium</li>
            <li>Stratégie marketing et positionnement différenciant</li>
            <li>Gestion complète expérience client et opérations</li>
          </ul>
          <div class="results-highlight">
            💎 ≈50K€/trimestre ⭐ Marque premium
          </div>
        </div>

        <div class="experience-card">
          <h3>DreamTeam Animation</h3>
          <div class="role">Directeur d'Animation Touristique</div>
          <div class="period">2018 – 2022</div>
          <ul>
            <li>Management de 25 animateurs / hôtel sur 5 établissements</li>
            <li>Stratégies d'animation à fort impact commercial</li>
            <li>Suivi satisfaction client et optimisation continue</li>
          </ul>
          <div class="results-highlight">
            💵 ≈25K€/saison 👥 125+ équipe
          </div>
        </div>
      </div>

      <!-- Formation -->
      <div class="content-section">
        <h2>🎓 Formation & Certifications</h2>

        <div class="formation-item">
          <h4>Graduate Assistant Commercial</h4>
          <div class="org">STUDI – En cours (2024-2025)</div>
        </div>

        <div class="formation-item">
          <h4>Andy Elliott – High-Performance Closing</h4>
          <div class="org">The Elliott Group – 2022</div>
        </div>

        <div class="formation-item">
          <h4>Sabri Suby – Sell Like Crazy</h4>
          <div class="org">Direct Response Marketing – 2022</div>
        </div>

        <div class="formation-item">
          <h4>Dean Graziosi – Mastermind</h4>
          <div class="org">Content Marketing Expert – 2022</div>
        </div>

        <div class="formation-item">
          <h4>Tourisme & Commerce</h4>
          <div class="org">École Monastir, Tunisie – 2015</div>
        </div>
      </div>

      <!-- Competences -->
      <div class="content-section">
        <h2>🎯 Compétences Validées DIAGORIENTE</h2>

        <div class="competences-grid">
          <div class="competence-category">
            <h4>💼 Business & Stratégie</h4>
            <ul>
              <li>Création d'entreprise & startup</li>
              <li>Élaborer stratégie commerciale</li>
              <li>Diagnostic stratégique</li>
              <li>Business plan & investissement</li>
              <li>Piloter performance & rentabilité</li>
            </ul>
          </div>

          <div class="competence-category">
            <h4>📊 Analyse & Data</h4>
            <ul>
              <li>Collecter et analyser données</li>
              <li>Analyser, structurer données</li>
              <li>Veille marché & concurrentielle</li>
              <li>Analyse comptable & financière</li>
              <li>Résolution problèmes complexes</li>
            </ul>
          </div>

          <div class="competence-category">
            <h4>🎯 Commercial & Client</h4>
            <ul>
              <li>Présenter & valoriser produit</li>
              <li>Convaincre, négocier</li>
              <li>Prospecter nouveaux marchés</li>
              <li>Développer relation client</li>
              <li>Actions commerciales & promo</li>
            </ul>
          </div>

          <div class="competence-category">
            <h4>👥 Management & Leadership</h4>
            <ul>
              <li>Animer réseau & communauté</li>
              <li>Préparer & animer réunions</li>
              <li>Inspirer, donner du sens</li>
              <li>Assistance technique équipes</li>
              <li>Organiser selon priorités</li>
            </ul>
          </div>
        </div>
      </div>

      <!-- CTA -->
      <div class="cta-section">
        <h2>CONTACTEZ-MOI MAINTENANT!</h2>
        <p style="font-size: 18px; margin-top: 10px;">Disponible pour une alternance immédiate</p>
        <div class="cta-buttons">
          <a href="tel:+33602560229" class="cta-btn">📞 APPELER</a>
          <a href="mailto:azerrached3@gmail.com" class="cta-btn">✉️ EMAIL</a>
        </div>
        <div class="social-links">
          <a href="https://www.tiktok.com/@thebrandnewdady" target="_blank">TikTok</a> •
          <a href="https://www.linkedin.com/in/azer-rached-239258377/" target="_blank">LinkedIn</a> •
          <a href="https://linktr.ee/AZER_rached" target="_blank">Linktree</a> •
          <a href="https://studi-connect.grimp.io/share?profile=JJ-8kzDBebDv" target="_blank">STUDI</a>
        </div>
      </div>

    </div>

  </div>

</div>

</body>
</html>
