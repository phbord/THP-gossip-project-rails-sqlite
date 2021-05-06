# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version : _5.2.5_

* System dependencies :
  * gem `table_print`
  * gem `faker`

* Deployment instructions
  * diagramme ERD : _db:/diagram_erd.vpd.pdf_
  * `bundle i`
  * `rails db:migrate`
  * `rails db:seed`

* Configuration

* Database creation
  * `rails generate model User first_name:string last_name:string describtion:text age:integer`
  * `rails generate model City name:string zip_code:string`
  * `rails generate model Gossip title:string content:text`
  * `rails generate model Tag title:string`
  * `rails generate model Comment content:text`
  * `rails generate model Like`
  * `rails generate model PrivateMessage content:text`

* Database initialization
  * `rails db:migrate`

* How to run the test suite

* Seeds
  * `rails db:seed`

* Tests

|ACTION|COMMANDE|
|:---|:---|
|||
|||
|||
|||
|||
|||
|||

## Schema de la Base de Données
[![](https://mermaid.ink/img/eyJjb2RlIjoiZXJEaWFncmFtXG4gICAgICAgIGNpdGllcyB8fC0tb3sgdXNlcnM6IGJlbG9uZ3NfdG9cbiAgICAgICAgY2l0aWVze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyBuYW1lXG4gICAgICAgIHN0cmluZyB6aXBfY29kZVxuICAgICAgICB9XG4gICAgICAgIHVzZXJzIHx8LS1veyBnb3NzaXBzOiBiZWxvbmdzX3RvXG4gICAgICAgIHVzZXJze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyBmaXJzdF9uYW1lXG4gICAgICAgIHN0cmluZyBsYXN0X25hbWVcbiAgICAgICAgdGV4dCBkZXNjcmlwdGlvblxuICAgICAgICBpbnRlZ2VyIGFnZVxuICAgICAgICBpbnRlZ2VyIGNpdHlfaWRfRktcbiAgICAgICAgfVxuICAgICAgICBnb3NzaXBze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyB0aXRsZVxuICAgICAgICB0ZXh0IGNvbnRlbnRcbiAgICAgICAgaW50ZWdlciB1c2VyX2lkX0ZLXG4gICAgICAgIGludGVnZXIgdGFnX2lkX0ZLXG4gICAgICAgIH1cbiAgICAgICAgdXNlcnMgfHwtLW97IHByaXZhdGVfbWVzc2FnZXM6IGJlbG9uZ3NfdG9cbiAgICAgICAgcHJpdmF0ZV9tZXNzYWdlc3tcbiAgICAgICAgaW50ZWdlciBpZF9QS1xuICAgICAgICB0ZXh0IGNvbnRlbnRcbiAgICAgICAgaW50ZWdlciBzZW5kZXJfaWQtVXNlcl9GS1xuICAgICAgICBpbnRlZ2VyIHJlY2lldmVyX2lkLVVzZXJfRktcbiAgICAgICAgfVxuICAgICAgICB1c2VycyB8fC0tb3sgY29tbWVudHM6IGJlbG9uZ3NfdG9cbiAgICAgICAgY29tbWVudHN7XG4gICAgICAgIGludGVnZXIgaWRfUEtcbiAgICAgICAgdGV4dCBjb250ZW50XG4gICAgICAgIGludGVnZXIgZ29zc2lwX2lkX0ZLXG4gICAgICAgIGludGVnZXIgdXNlcl9pZF9GS1xuICAgICAgICB9XG4gICAgICAgIGdvc3NpcHMgfHwtLW97IGxpa2VzOiBiZWxvbmdzX3RvXG4gICAgICAgIGxpa2Vze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIGludGVnZXIgZ29zc2lwc19pZF9GS1xuICAgICAgICBpbnRlZ2VyIHVzZXJfaWRfRktcbiAgICAgICAgaW50ZWdlciBjb21tZW50X2lkX0ZLXG4gICAgICAgIH1cbiAgICAgICAgY29tbWVudHMgfHwtLW97IGxpa2VzOiBiZWxvbmdzX3RvXG4gICAgICAgIHVzZXJzIHx8LS1veyBsaWtlczogYmVsb25nc190b1xuICAgICAgICB0YWdzIHx8LS1veyBnb3NzaXBzOiBiZWxvbmdzX3RvXG4gICAgICAgIHRhZ3N7XG4gICAgICAgIGludGVnZXIgaWRfUEtcbiAgICAgICAgc3RyaW5nIHRpdGxlXG4gICAgICAgIH0iLCJtZXJtYWlkIjp7fSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZXJEaWFncmFtXG4gICAgICAgIGNpdGllcyB8fC0tb3sgdXNlcnM6IGJlbG9uZ3NfdG9cbiAgICAgICAgY2l0aWVze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyBuYW1lXG4gICAgICAgIHN0cmluZyB6aXBfY29kZVxuICAgICAgICB9XG4gICAgICAgIHVzZXJzIHx8LS1veyBnb3NzaXBzOiBiZWxvbmdzX3RvXG4gICAgICAgIHVzZXJze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyBmaXJzdF9uYW1lXG4gICAgICAgIHN0cmluZyBsYXN0X25hbWVcbiAgICAgICAgdGV4dCBkZXNjcmlwdGlvblxuICAgICAgICBpbnRlZ2VyIGFnZVxuICAgICAgICBpbnRlZ2VyIGNpdHlfaWRfRktcbiAgICAgICAgfVxuICAgICAgICBnb3NzaXBze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIHN0cmluZyB0aXRsZVxuICAgICAgICB0ZXh0IGNvbnRlbnRcbiAgICAgICAgaW50ZWdlciB1c2VyX2lkX0ZLXG4gICAgICAgIGludGVnZXIgdGFnX2lkX0ZLXG4gICAgICAgIH1cbiAgICAgICAgdXNlcnMgfHwtLW97IHByaXZhdGVfbWVzc2FnZXM6IGJlbG9uZ3NfdG9cbiAgICAgICAgcHJpdmF0ZV9tZXNzYWdlc3tcbiAgICAgICAgaW50ZWdlciBpZF9QS1xuICAgICAgICB0ZXh0IGNvbnRlbnRcbiAgICAgICAgaW50ZWdlciBzZW5kZXJfaWQtVXNlcl9GS1xuICAgICAgICBpbnRlZ2VyIHJlY2lldmVyX2lkLVVzZXJfRktcbiAgICAgICAgfVxuICAgICAgICB1c2VycyB8fC0tb3sgY29tbWVudHM6IGJlbG9uZ3NfdG9cbiAgICAgICAgY29tbWVudHN7XG4gICAgICAgIGludGVnZXIgaWRfUEtcbiAgICAgICAgdGV4dCBjb250ZW50XG4gICAgICAgIGludGVnZXIgZ29zc2lwX2lkX0ZLXG4gICAgICAgIGludGVnZXIgdXNlcl9pZF9GS1xuICAgICAgICB9XG4gICAgICAgIGdvc3NpcHMgfHwtLW97IGxpa2VzOiBiZWxvbmdzX3RvXG4gICAgICAgIGxpa2Vze1xuICAgICAgICBpbnRlZ2VyIGlkX1BLXG4gICAgICAgIGludGVnZXIgZ29zc2lwc19pZF9GS1xuICAgICAgICBpbnRlZ2VyIHVzZXJfaWRfRktcbiAgICAgICAgaW50ZWdlciBjb21tZW50X2lkX0ZLXG4gICAgICAgIH1cbiAgICAgICAgY29tbWVudHMgfHwtLW97IGxpa2VzOiBiZWxvbmdzX3RvXG4gICAgICAgIHVzZXJzIHx8LS1veyBsaWtlczogYmVsb25nc190b1xuICAgICAgICB0YWdzIHx8LS1veyBnb3NzaXBzOiBiZWxvbmdzX3RvXG4gICAgICAgIHRhZ3N7XG4gICAgICAgIGludGVnZXIgaWRfUEtcbiAgICAgICAgc3RyaW5nIHRpdGxlXG4gICAgICAgIH0iLCJtZXJtYWlkIjp7fSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)
## Projet
- poser les bases de _Gossip Project_ pour le transcrire en Rails
- modéliser la BDD
- parcours utilisateur (s'inscrire)
  - prénom
  - nom
  - mail
  - age
  - ville
  - code postal
- fonctionnalités
  - créer des potins
  - mettre un ou plusieurs tags sur les potins : #romance (sur les potins)
  - commenter des potins
  - commenter des commentaires
  - liker des potins
  - contacter leur commères favoris en MP
- rechercher les potins par :
  - ville
  - utilisateurs
  - date (plus récent ou plus ancien)
  - nombre de likes
  - tags

### Diagrammes ERD

### Models
- User
- City
- Gossip
- Tag
- PrivateMessage
- Comment
- like
- commentaire de commentaires en `polymorphism`
