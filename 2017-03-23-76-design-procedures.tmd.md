---
title: 76-design-procedures.tmd
layout: post
author: coderoller
permalink: /76-design-procedures.tmd/
source-id: 1B3fL_pL87QAkCHeaKEMZWYK1cRHvGZ8nP8VXS83RENw
published: true
---
# 76Design Procedures

## connect to test server

ssh echlin@ssh.dev.76engage.com

Engage root is: /home/engage/public_html 

## Update process

Update locally

1 Update existing git repo of 76Engage on your computer

1 Run the site

1 View the site, make sure it is working

1 Log in to site:

  * support@76design.com

  * JsMzR9omkR7q (for core Engage at this time only)

1 Look at: Modules/Update

1 Ignore modules that have a version ending in -dev-dev

  * These are modules that are pinned to a specific Git version for now.

1 Modify the corresponding entry for the module, in engage.make, to the "Recommended version"

1 Run the following command:

  * > ./vendor/bin/drush -y make engage.make

  * This will copy all the PHP modules from their source locations to this installation

1 View in web server

1 Git commit engage.make, when that file is working

Update on test server

1 ssh to that server

  * ssh echlin@ssh.dev.76engage.com

  * replace "echlin" with your id on that machine

1 git pull, this should update engage.make

1 restart nginx on ssh.dev.76engage.com

1 view the site on 

## Metrolinx credentials for now

* https://www.metrolinxengage.com/en/user

* support@76design.com

* Password - not recorded here

Deploy by ssh:

* (machine?)

* tfadmin

* password not recorded here

## SDTC.ca

* user: sdtc

* machine?

* transport/connection method?

