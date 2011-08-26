---
title: Pour commencer
kind: content
---

<h3>Pré-requis</h3>

Votre dépot doit avoir un Rakefile dont la tâche par défault (`default`) est une tâche de test. C'est tout. Travis CI va exécuter `bundle install` si le projet a un Gemfile, puis `rake` par défaut.

Vous pouvez <a href="/fr/docs/user/build-configuration/">configurer</a> tout cela, y compris les <a href="/fr/docs/user/database-setup/">connexions aux bases de données</a>.

<h3>Se connecter</h3>

Connectez-vous avec Github en cliquant sur le lien `Sign in with Github` sur <a href="http://travis-ci.org">la page d'accueil de Travis CI</a>.

Github va vous demander d'accorder à Travis CI des droits d'accès en lecture et en écriture. Travis CI a besoin d'accès en écriture seulement pour activer automatiquement les hooks quand vous configurez un projet, mais il ne touchera rien d'autre.

<h3>Ajouter les hooks</h3>

Une fois connecté, allez sur <a href="http://travis-ci.org/profile">votre page de profil</a>. Vous y verrez une liste de vos dépots où vous pouvez activer les dépots que vous voulez tester avec Travis CI.

Cliquez sur la clé pour visiter la page des hooks de votre projet Github. Vous pouvez y configurer l'utilisateur Github utilisé par Travis CI.

<h3>Déclenchement d'une build</h3>

Pour démarrer une build, vous pouvez soit pusher un commit vers votre dépot Github, ou aller sur la page des hooks sur Github et utiliser le bouton "Test Hook" dans les préférences du hook Travis.

Si tout va bien cela devrait insérer un job dans la file d'attente de <a href="http://travis-ci.org">Travis CI</a>. Votre build commencera dès qu'un worker sera disponible.

<h3>Configurer votre build</h3>

Vous pouvez configurer votre build en ajouter un fichier `.travis.yml` à la racine de votre dépot. Voir <a href="/docs/user/build-configuration/">Configurer une build</a>.

<h3>Plus de détails sur l'infrastructure disponible</h3>

Un worker contient un grand nombre de services utilisés couramment, comme MySQL, PostgreSQL, MongoDB, memcached et beaucoup d'autres.

Voir <a href="/fr/docs/user/database-setup/">Database setup</a> pour plus de détails sur la configuration d'une base de données pour votre suite de tests.

<h3>Besoin d'aide ?</h3>

Pour toutes questions, connectez vous sur notre channel IRC <a href="irc://irc.freenode.net#travis">#travis sur irc.freenode.net</a>. Attention, la plupart des contributeurs ne parlent pas français, présenter votre problème en anglais serait préférable.
