# Vagrant DNS Lab - репозиторий для развёртывания лабораторного стенда по выполненному ДЗ со сконфигурированным Split-DNS

Для развёртываний используйте команды:

```
git clone https://github.com/kosogoroff/vagrant-bind.git
cd vagrant-bind
vagrant up
```

Для создания репозитория использовались команды:

```
[admin_insta11@mv334 vagrant-bind]$ git init
подсказка: Using 'master' as the name for the initial branch. This default branch name
подсказка: is subject to change. To configure the initial branch name to use in all
подсказка: of your new repositories, which will suppress this warning, call:
подсказка: 
подсказка: 	git config --global init.defaultBranch <name>
подсказка: 
подсказка: Names commonly chosen instead of 'master' are 'main', 'trunk' and
подсказка: 'development'. The just-created branch can be renamed via this command:
подсказка: 
подсказка: 	git branch -m <name>
Инициализирован пустой репозиторий Git в /home/admin_insta11/vagrant-bind/.git/
[admin_insta11@mv334 vagrant-bind]$ 
[admin_insta11@mv334 vagrant-bind]$ git add .
[admin_insta11@mv334 vagrant-bind]$ 
[admin_insta11@mv334 vagrant-bind]$ git commit -m "first commit"
[master (корневой коммит) ef4921d] first commit
 16 files changed, 445 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 Vagrantfile
 create mode 100644 provisioning/client-motd
 create mode 100644 provisioning/client-resolv.conf
 create mode 100644 provisioning/master-named.conf
 create mode 100644 provisioning/named.ddns.lab
 create mode 100644 provisioning/named.dns.lab
 create mode 100644 provisioning/named.dns.lab.rev
 create mode 100644 provisioning/named.newdns.lab
 create mode 100644 provisioning/named.zonetransfer.key
 create mode 100644 provisioning/playbook.yml
 create mode 100644 provisioning/rndc.conf
 create mode 100644 provisioning/servers-resolv.conf.j2
 create mode 100644 provisioning/slave-named.conf
 create mode 100644 provisioning/zonetransfer.key
[admin_insta11@mv334 vagrant-bind]$ 
[admin_insta11@mv334 vagrant-bind]$ git branch -M main
[admin_insta11@mv334 vagrant-bind]$ 
[admin_insta11@mv334 vagrant-bind]$ git remote add origin https://github.com/kosogoroff/vagrant-bind.git
[admin_insta11@mv334 vagrant-bind]$ 
[admin_insta11@mv334 vagrant-bind]$ git push -u origin main

(gnome-ssh-askpass:397915): dbind-WARNING **: 20:27:40.885: Couldn't connect to accessibility bus: Empty address ''

(gnome-ssh-askpass:397932): dbind-WARNING **: 20:27:45.566: Couldn't connect to accessibility bus: Empty address ''
Перечисление объектов: 18, готово.
Подсчет объектов: 100% (18/18), готово.
При сжатии изменений используется до 24 потоков
Сжатие объектов: 100% (17/17), готово.
Запись объектов: 100% (18/18), 4.65 КиБ | 953.00 КиБ/с, готово.
Total 18 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/kosogoroff/vagrant-bind.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
[admin_insta11@mv334 vagrant-bind]$ 


```
