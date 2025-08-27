---
layout: default
title: "Home"
---

<section id="about" class="section-box rounded-3xl p-10 mb-16">
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
            I have been an Associate Professor at 
            <a href="https://www.univ-lyon2.fr/" class="gold-link"  target="_blank">Université Lumière Lyon 2</a> 
            since September 2023. I am in charge of the program 
            "Visualization, Design of Decision-Making Tools" within the  
            <a href="https://iut.univ-lyon2.fr/formations/but/but-science-des-donnees/" class="gold-link"  target="_blank">Data Science Department at IUT Lumière</a>, 
            where I teach Python programming, NoSQL databases, the migration from relational to non-relational data, Big Data and Advanced Big Data, as well as Data Security. 
            I am a member of the SID team of the research unit  
            <a href="https://eric.msh-lse.fr/"  class="gold-link" target="_blank">ERIC</a>. 
            My main research interests are related to data management (Big Data, Data Lakes, Polystores, vector databases), data sharing, data analysis, and data security.
          </p>
        </div>
    </div>
</section>

<section id="research" class="section-box rounded-3xl p-10 mb-16">
  <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4">Research Interests</h2>
  <ul class="list-disc list-inside">
    <li>Data management (Big Data, Data Lakes, Polystores...)</li>
    <li>Data sharing and security</li>
    <li>Health data analysis</li>
    <li>Explainability</li>
  </ul>
</section>

<section id="publications" class="section-box rounded-3xl p-10 mb-16">
  <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
    Publications et Projets
  </h2>
  <div class="space-y-8 text-lg">
    {% assign pubs = site.data.publications | sort: "year" | reverse %}
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
</section>

<section id="teaching" class="section-box rounded-3xl p-10 mb-16">
    <h2 class="text-4xl font-bold text-accent mb-8 border-b-2 border-accent pb-4 flex items-center">
        <!-- Icon for the "Teaching" section -->
        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 mr-4 text-accent" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4"></path><path d="M10 2c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4"></path><path d="M6 2c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4c.8 1.1 1.2 2.5 1.2 4s-.4 2.9-1.2 4"></path><path d="M18 2c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4c-.8 1.1-1.2 2.5-1.2 4s.4 2.9 1.2 4"></path><path d="M22 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M16 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M12 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M8 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M2 22h-4c-1.1 0-2 .9-2 2v0"></path><path d="M18 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M14 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M10 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M6 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M2 2h-4c-1.1 0-2 .9-2 2v0"></path><path d="M20 2v20"></path><path d="M4 2v20"></path></svg>
        Teaching
    </h2>
    <div class="space-y-8 text-lg">
        <!-- Courses organized by level -->
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Undergraduate</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
                <li>Algorithms and data structures</li>
                <li>Object-oriented programming with Java</li>
                <li>Web programming (PHP, HTML, CSS, JavaScript)</li>
                <li>Databases for the web (SQL)</li>
            </ul>
        </div>
        <div class="p-6 rounded-xl border-2 border-gray-700 hover:border-accent transition-colors duration-300">
            <h3 class="font-semibold text-xl mb-2 text-accent">Graduate</h3>
            <ul class="list-disc list-inside space-y-1 text-gray-400">
                <li>Big Data and visualization (Hadoop, Spark, Kafka)</li>
                <li>Web application development with containerization (Docker)</li>
                <li>Non-relational databases (MongoDB, Neo4J, Cassandra, Redis)</li>
                <li>Data analysis (Pandas, GGplot)</li>
                <li>Information systems security (Access control, Anonymization, IT Risk Management with EBIOS)</li>
                <li>Software engineering (Design patterns, Git, GitLab CI/CD)</li>
            </ul>
        </div>
    </div>
</section>
