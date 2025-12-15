EXERCICE 1: MANIPULATION DES BRANCHES LOCALEMENT
Initialisation du projet:
git init
echo "<p>Lorem ipsum...</p>" > index.html
git add index.html
git commit -m "Initial commit"
Branche fn/tab:
git checkout -b fn/tab
Modifier index.html
git add index.html
git commit -m "Feat: Ajout titre et tableau"
Branche fn/footer:
git checkout master
git checkout -b fn/footer
Modifier index.html
git add index.html
git commit -m "Feat: Ajout footer"
Fusion fn/footer dans fn/tab:
git checkout fn/tab
git merge fn/footer
Resoudre les conflits dans index.html
git add index.html
git commit -m "Merge: Fusion de fn/footer dans fn/tab"
Fusion fn/tab dans master:
git checkout master
git merge fn/tab


EXERCICE 2: GIT / GITHUB
Creer projet GitHub: Via l'interface web.
Cloner le projet:
git clone <URL_DU_REPO>
cd <NOM_DU_REPO>
Ajouter default.html:
echo "<h1>Contenu HTML</h1>" > default.html
Ajouter et valider:
git add default.html
git commit -m "feat: Ajout default.html"
Push vers le distant:
git push origin main
Modifier le fichier sur GitHub: Via l'interface web.
Pull les modifications en local:
git pull origin main
Creer une branche locale design:
git checkout -b design
Ajouter style.css et lier:
Creer style.css et modifier default.html
Ajouter et valider:
git add .
git commit -m "feat: Ajout style"
Push la nouvelle branche:
git push -u origin design
Accepter la fusion: Via une "Pull Request" sur GitHub.


EXERCICE 3
Afficher le contenu: ls | Resultat: cours/ git.txt scrum.txt
Enregistrer et valider: git add . puis git commit -m "message"
Creer la branche "activites": git checkout -b activites
Afficher les branches: git branch
Afficher l'historique: git log


EXERCICE 4
Resultat de ls: projects/ readme.md
Creer le dossier devowfs: mkdir devowfs puis cd devowfs
Role de git config: Configure le nom de l'auteur pour les commits.
Initialiser git dans devowfs: git init
Ajouter et valider note.txt: git add note.txt puis git commit -m "message"
Creer et lister une branche: git branch <nom_branche> puis git branch
Placer HEAD sur la nouvelle branche: git checkout <nom_branche>


EXERCICE 5
Repertoire de travail -> Index git:
git add <nom_du_fichier>
Index git -> Repertoire Local:
git commit -m "message"
Repertoire Local -> Repertoire Distant:
git push
Repertoire Distant -> Repertoire de travail:
git pull
