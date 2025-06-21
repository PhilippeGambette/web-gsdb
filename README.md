# web-gsdb
Un outil de déploiement de site web à partir d'une base de données stockée sur Google Sheets.

## Démos

* Site créé par [Olivier Brossard](https://www.iufrance.fr/les-membres-de-liuf/membre/1507-olivier-brossard.html) : [Bibliographie de poésie des États-Unis en traduction française, 1786-2023](https://philippegambette.github.io/web-gsdb/?id=poesie-americaine-en-traduction)
* Site de [recensement des promenades du matrimoine en France](https://philippegambette.github.io/web-gsdb/?id=empreintes-de-femmes) (données collectées par Danie Lancéa, Titouan Kerhervé-Remoussin et Philippe Gambette)
* Site créé par [Beatrice Mundo](https://digis.hypotheses.org/1526) : [Lettres de Catherine de Médicis 1564-1566](https://beatricemundo.github.io/lettresmedicis6466/)

## Installation

* Copiez les fichiers de ce dépôt dans un dossier pris en compte par le serveur web.
* Créez un fichier texte, avec un code inspiré du code JSON ci-dessous, pour préciser les informations affichées sur le site ainsi que l'URL source des données du site (pour trouver cette URL à partir de votre fichier Google Sheets,  menu "Fichier", "Partager", "Publier sur le web", puis dans la fenêtre qui apparait, choisis non pas "Document entier" mais la feuille souhaitée, et dans la liste déroulante juste à droite choisir le format "valeurs séparées par des virgules (csv)" et cliquer sur "Publier" pour récupérer l'URL qui apparait alors)
* Enregistrez ce fichier texte sous le nom `infos-nom_que_vous_avez_choisi.json`, à l'intérieur du dossier où vous avez copié les autres fichiers
* Le site est alors consultable à l'adresse http://votre_nom_de_domaine.com/votre_dossier/?id=nom_que_vous_avez_choisi

Exemple de code JSON, pour un site web dédié aux promenades du matrimoine en France :
`{"url":"https://docs.google.com/spreadsheets/d/e/2PACX-1vTeCq1Aa8gVJfDOH38noAGKODRVmHsZkh8bElJmBZDKZygs8sORJ1NLXUgq8AApXo4JpIGbMsylQQHS/pub?gid=0&single=true&output=csv","credits":["<p style=\"font-size:1.5em\">Données collectées par Danie Lancéa, Titouan Kerhervé-Remoussin et Philippe Gambette, pour le projet <a href=\"http://citedesdames.hypotheses.org\">Cité des dames, créatrices dans la cité</a>.</p>"],"title":["Empreintes de femmes : recensement des promenades du matrimoine en France"],"image":["src","https://citedesdames.github.io/empreintesdefemmes/assets/img/logo-epais.png"],"fields":["titre","ville","adresse","liste_femmes","URL","date","régularité","lat","long","est_numerique"]}`

## Pour aller plus loin

* pour des sites web ou des bases de données plus complexes, vous pouvez utiliser [Awesome Table](https://awesome-table.com/)
* d'autres moteurs de sites créés à partir de fichiers Google Sheets par des stagiaires à l'université Gustave Eiffel :
  * [De ville en ville](https://github.com/citedesdames/de-ville-en-ville)
  * [Les Promenades du Matrimoine](https://github.com/Ulysseee/les-promenades-du-matrimoine)
  * [Empreintes de femmes](https://github.com/citedesdames/empreintesdefemmes)
