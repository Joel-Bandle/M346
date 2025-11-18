# HN01

## Hypervisor Typ 1
Der Hypervisor vom Typ 1 sitzt auf dem Bare Metal Server und hat direkten Zugriff auf die Hardware-Ressourcen.

## Hypervisor Typ 2
Der Typ-2-Hypervisor ist eine Anwendung, die auf dem Host-Betriebssystem installiert ist.

## Unterschied
Der Hauptunterschied ist, dass Hypervisoren vom Typ 1 direkt auf der Hardware laufen und keine darunterliegende Betriebssystemschicht benötigen, während Hypervisoren vom Typ 2 als Anwendung auf einem bestehenden Host-Betriebssystem installiert werden.

## Vermutung
(Ich habe Hyper V benutzt)
Ich glaube es lauft auf den Hypervisor Typ 1 da es Information und direkten Zugriff aud die Hardware-Ressourcen hat.

## Warum die Zuweisung von mehr logischen Prozessoren oder RAM nicht funktioniert
Die Zuordnung von logischen Prozessoren oder RAM zu einer virtuellen Maschine muss innerhalb der physischen Grenzen des Host-Systems liegen. Wenn man mehr Ressourcen zuweisen, als tatsächlich vorhanden sind, kommt es zu folgenden Problem:

Die Anzahl der logischen Prozessoren oder der verfügbare RAM übersteigt die physische Kapazität. Der Hypervisor kann keine nicht vorhandenen Ressourcen bereitstellen.