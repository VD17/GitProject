# GitProject

Dans le cadre de notre projet git nous devions signer chacun de nos commit des étapes sont indispensable telle que la génération de notre clé GPG & SSH

## Générer une nouvelle paire de clés
gpg --full-generate-key

1 - 4096 - 0 - y - <prenom.nom> - <mail git> - Auto-sign - O - Ignorer le champs passphrase > yes no need protection

## Voir la liste de toutes les clés GPG
gpg --list-keys

## Exporter la clé publique
gpg --armor --export <ID de la clé>

## Configurer Git pour utiliser GPG
git config --global user.signingkey <ID de la clé>
git config --global commit.gpgsign true

---------------------

## Configurer Git pour utiliser SSH

ssh-keygen -t ed25519  -C " "
cat /home/vishal/.ssh/id_ed25519.pub\n
git clone git@github.com:tgelectro/Projet_GIT.git

---------------------

## Pour faire une branch et aller durectement sur celle-ci

git checkout -b Branch-By-Vishal
git push <- pour bien partager la branch au collaborateur

---------------------

## Afin de crée des issue nous utiliserons le packet "gh" ce dernier s'installe ainsi

sudo apt install gh

gh issue create --title "My new issue" --body "Here are more details."

gh issue create --title "My new issue" --body "Here are more details." --assignee @me,monalisa --label "bug,help wanted" --project onboarding --milestone "learning codebase"

---------------------

