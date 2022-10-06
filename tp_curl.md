# TP curl - comprendre les requêtes et les réponses HTTP

Pour les questions suivantes, vous devez utiliser l'url suivante : https://webhook.site/6f594809-a4b4-483e-841b-0c3b0a00edfe

Pour tous les appels vous devez ajouter un header pour identifier votre appel parmis ceux des autres étudiants : x-student : VOTRE_NOM

## Faire un appel curl : copier la commande exécutée et indiquer la requête et la réponse
curl -v --header "x-student:ZAROUKI Hamza" https://webhook.site/d4ec90aa-8173-48dd-8414-6fb832ea2a26

*   Trying 46.4.105.116:443...
* Connected to webhook.site (46.4.105.116) port 443 (#0)
* schannel: ALPN, offering http/1.1
* ALPN, server did not agree to a protocol
> GET /d4ec90aa-8173-48dd-8414-6fb832ea2a26 HTTP/1.1
> Host: webhook.site
> User-Agent: curl/7.71.1
> Accept: */*
> x-student:ZAROUKI Hamza
>
* Mark bundle as not supporting multiuse
< HTTP/1.1 200 OK
< Server: nginx
< Content-Type: text/plain; charset=UTF-8
< Transfer-Encoding: chunked
< Vary: Accept-Encoding
< X-Request-Id: c4cef73b-79c2-45f0-a3fb-bee9c85013ad
< X-Token-Id: d4ec90aa-8173-48dd-8414-6fb832ea2a26
< Cache-Control: no-cache, private
< Date: Thu, 22 Sep 2022 12:41:00 GMT
<
* Connection #0 to host webhook.site left intact

## Quel est la version du protocole utilisé par le serveur ?
HTTP/1.1

## Quels sont les headers que l'on envoie dans la requête ? Quels sont leur sens ?
> Accept: */*
> Host: webhook.site
> User-Agent: curl/7.71.1
< HTTP/1.1 200 OK
< Content-Type: text/plain; charset=UTF-8
< Vary: Accept-Encoding
< X-Request-Id: c4cef73b-79c2-45f0-a3fb-bee9c85013ad
< X-Token-Id: d4ec90aa-8173-48dd-8414-6fb832ea2a26
< Cache-Control: no-cache, private
< Date: Thu, 22 Sep 2022 12:41:00 GMT

HTTP/1.1: version protocole HTTP.
200 OK: code de statut. le serveur a reçu, compris et accepté la demande.
Content-Type: fournit des informations sur le type de fichier.
Cache-Control, Vary: référence à la mise en cache du fichier.
server: désigne le logiciel du serveur Web.
Accept: types de contenu que le client peut traiter
Date: date et heure de la demande

## Quelles informations pouvez-vous trouver à propos du certificat SSL ?
SSL certificate verify ok

## Quel est le code de la réponse ? Que signifie-t-il ?
< Server: nginx
< Vary: Accept-Encoding
< Transfer-Encoding: chunked
> GET /d4ec90aa-8173-48dd-8414-6fb832ea2a26 HTTP/1.1

server: Identification du serveur
vary: Indique quels champs d’en-tête doivent être considérés comme variables si un fichier est demandé dans le cache
Transfer-Encoding: Méthode de compression
GET: allow: Types de demandes autorisées pour une ressource spécifique

## Quels headers recevez vous dans la response ? Quels sont leur sens ?


## Faire un appel curl en envoyant du texte brut : copier la commande exécutée et indiquer la requête et la réponse


## Faire un appel curl en envoyant du JSON (avec les bons headers) : copier la commande exécutée et indiquer la requête et la réponse


## Faire une appel curl en envoyant une basic authentication en utilisant 2 méthodes différentes : copier les commandes exécutées et indiquer la requête et la réponse à chaque fois 


## Exécuter la commande suivante avec la méthode GET puis indiquer la réponse : curl https://demo.api-platform.com/books/07dd4786-aaa7-4d08-a467-076b76f1d1b6 


## Exécuter la commande suivante avec la méthode PATCH  puis indiquer la réponse : curl https://demo.api-platform.com/top_books/1


## Quel est le code HTTP reçu ? Quel est sa signification ?


## Exécuter la commande suivante puis indiquer la réponse : curl https://demo.api-platform.com/top_books/1


## Exécuter la commande suivante puis indiquer la réponse : curl https://demo.api-platform.com/top_books/9999


## Quel est le code HTTP ? Que signifie-t-il ?


## Exécuter la requête suivante et copier la réponse : curl https://google.fr


## Quel est le code HTTP reçu ? Pouvez-vous expliquer cette réponse ?


## Comment éviter cette réponse ? Trouvez 2 solutions différentes et détaillez les.
