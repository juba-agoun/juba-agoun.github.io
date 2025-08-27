---
layout: default
title: "Accueil"
---

<section id="apropos" class="section-box rounded-3xl p-10 mb-16">
    <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
        <!-- Icône utilisateur pour la section "À propos" -->
        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 mr-4 text-accent" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
        À propos de moi
    </h2>
    <div class="flex flex-col md:flex-row items-center space-y-8 md:space-y-0 md:space-x-12">
        <div class="md:w-1/4 flex justify-center">
            <!-- Utilisation d'une image de remplacement pour la photo de profil -->
            <img src="../img/juba-agoun.jpg" alt="Photo de profil de Juba Agoun" class="rounded-full border-4 border-gray-700 w-64 h-64 object-cover shadow-2xl">
        </div>
        <div class="md:w-3/4 text-lg leading-relaxed space-y-4">
          <p>
            Je suis enseignant-chercheur à 
            <a href="https://www.univ-lyon2.fr/" class="gold-link" target="_blank">l'Université Lumière Lyon 2</a> 
            depuis septembre 2023. Je suis responsable du parcours 
            "Visualisation, Conception d'Outils Décisionnels" au sein du  
            <a href="https://iut.univ-lyon2.fr/formations/but/but-science-des-donnees/"  class="gold-link" target="_blank">département Data Science de l'IUT Lumière</a>, 
            où j'enseigne la programmation Python, les bases de données NoSQL, la migration de données relationnelles à non-relationnelles, le Big Data et le Big Data avancé, ainsi que la sécurité des données. 
            Je suis membre de l'équipe SID de l'unité de recherche 
            <a href="https://eric.msh-lse.fr/" class="gold-link" target="_blank">ERIC</a>. 
            Mes principaux intérêts de recherche sont liés à la gestion des données (Big Data, Datalakes, Polystores, bases de données vectorielles), au partage de données, à l'analyse de données et à la sécurité des données.
          </p>
        </div>
    </div>
</section>

<section id="recherche" class="section-box rounded-3xl p-10 mb-16">
  <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
      <!-- Icône d'ampoule pour la section "Recherche" -->
      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 mr-4 text-accent" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M15 14c.2-1 .7-1.7 1.5-2.5 1-.9 1.5-2.2 1.5-3.5A6 6 0 0 0 6 8c0 1.3.5 2.6 1.5 3.5.8.8 1.3 1.5 1.5 2.5"></path><path d="M9 18h6"></path><path d="M10 22h4"></path><path d="M8 22h8"></path><path d="M12 14v8"></path></svg>
      Intérêts de recherche
  </h2>
  <ul class="list-disc list-inside">
    <li>Gestion de données (Big Data, Datalakes, Polystores...)</li>
    <li>Partage de données et sécurité</li>
    <li>Analyse de données de santé</li>
    <li>Explicabilité</li>
  </ul>
</section>

<section id="publications" class="section-box rounded-3xl p-10 mb-16">
  <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
    Publications et Projets
  </h2>
 
  <div class="space-y-8 text-lg">
    {% assign pubs = site.data.publications | sort: "year" | reverse | slice:0,4 %}
    {% for pub in pubs %}
      <article class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
        <h3 class="font-semibold text-xl mb-2">{{ pub.title }}</h3>
        <p class="italic text-gray-400">{{ pub.authors }} — {{ pub.year }}</p>
        <p class="mt-2 text-sm">{{ pub.venue }}</p>
        {% if pub.link %}
          <a href="{{ pub.link }}" target="_blank" class="text-red-500">Lire</a>
        {% endif %}
      </article>
    {% endfor %}
  </div>
  <br>
  <h3 class="font-semibold text-xl mb-2 ">Retrouvez toutes mes publications sur mon <a href="https://scholar.google.com/citations?hl=fr&user=pT-ZQfIAAAAJ&view_op=list_works&sortby=pubdate"  class="gold-link" target="_blank"> ⚡Google Scholar⚡</a>
  </h3> 
</section>


<section id="enseignement" class="section-box rounded-3xl p-10 mb-16">
    <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
        <!-- Icône de tableau pour la section "Enseignement" -->
        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 mr-4 text-accent" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4"></path><path d="M10 2c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4"></path><path d="M6 2c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4"></path><path d="M18 2c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4"></path><path d="M22 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M16 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M12 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M8 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M2 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M18 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M14 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M10 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M6 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M2 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M20 2v20"></path><path d="M4 2v20"></path></svg>
        Enseignement
    </h2>
    <div class="space-y-8 text-lg">
        <!-- Détails des cours extraits du CV, organisés par niveau -->
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Licence</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
                <li>Algorithmique et structures de données</li>
                <li>Programmation orientée objet avec Java</li>
                <li>Programmation web (PHP, HTML, CSS, JavaScript)</li>
                <li>Bases de données pour le web (SQL)</li>
            </ul>
        </div>
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Master</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
                <li>Big Data et visualisation (Hadoop, Spark, Kafka)</li>
                <li>Développement d'applications web avec conteneurisation (Docker)</li>
                <li>Bases de données non relationnelles (MongoDB, Neo4J, Cassandra, Redis)</li>
                <li>Analyse de données (Pandas, GGplot)</li>
                <li>Sécurité des systèmes d'information (Contrôle d'acces, Anonymisation, IT Risk managment avec EBIOS)</li>
                <li>Ingénierie logicielle (Design patterns, Git, GitLab CI/CD)</li>
            </ul>
        </div>
    </div>
</section>




<section id="projets" class="section-box rounded-3xl p-10 mb-16">
    <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">      
        Projets
    </h2>
    <div class="space-y-8 text-lg">
        <!-- procjects organized by time-->
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Ongoing</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
                <li>AUTONOM-HEALTH - Health, behaviors and autonomous digital technologies 
                <a href="https://anr.fr/ProjetIA-22-PESN-0009"  class="gold-link" target="_blank">Voir plus</a> 
                </li>
                <li>Theoretical Framework for Designing and Analyzing Resilient Smart Cyber Systems
                <a href="https://rscs-fr-us.projet.liris.cnrs.fr/"  class="gold-link" target="_blank">Voir plus</a> 
                </li>
                <li>DataLAC : Données, Archives et Textes Archéologiques
                <a href="https://anr.fr/Projet-ANR-24-CE54-1690"  class="gold-link" target="_blank">Voir plus</a> 
                </li>
            </ul>
        </div>
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Past</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
              <li>Monitoring multidimensional aspects of QUAlity of Life after cancer ImmunoTherapy - an Open smart digital Platform for personalized prevention and patient management
                  <a href="https://cordis.europa.eu/project/id/875171"  class="gold-link" target="_blank">Voir plus</a> 
              </li>
              <li>Cyberspace Threat Identification, Analysis and Proactive Response
                  <a href="https://projet.liris.cnrs.fr/cyber/workshops.html"  class="gold-link" target="_blank">Voir plus</a> 
              </li>
              </ul>
        </div>
    </div>
</section>