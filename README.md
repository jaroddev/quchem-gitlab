# quchem-gitlab

## Présentation du projet
Ce repository git fait partie du projet QuChemPedIA2020 et a pour but stocker les fichiers ansible pour installer Gitlab-CE.
Ce répository a était créer dans l'optique de proposer gitlab comme coeur de l'infrastructure CI CD du projet principale.

Vous devriez pouvoir accéder au projet via l'url suivante: http://quchempedia.univ-angers.fr:8088/

## première visite après l'installation

Pensez a immédiatement changer le mot de passe administrateur, pour vous connecter la première fois:
- identifiant: root
- mot de passe: variable définie dans le playbook

## Avertissement

L'installation a était conçu pour une machine debian, dans le cas ou vous souhaiteriais customiser l'installation, je vous invite à consulter les liens suivants:
- ansible-role-gitlab by geerlingguy -> https://github.com/geerlingguy/ansible-role-gitlab
- la doc officielle de gitlab adéquate, faite attention à la version -> https://docs.gitlab.com/ce/install/

## Ansible

### version

Attention, ce projet fonctionne avec ansible 2.9.12 et n'a pas était testé avec les versions 2.10 et ultérieurs

### Variables ansible - customiser l'installation

- gitlab_external_url: URL à laquelle http://quchempedia.univ-angers.fr:8088
- gitlab_admin_password: Mot de passe par défaut de l'admin root gitlab
