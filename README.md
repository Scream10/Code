# Lucca | Chatbox 💻

Lien héberger sur Vercel : [ici](https://code-inky.vercel.app/)

## Contexte

Un chef de produit vient vous voir pour créer une page de chat dans son produit. Son fonctionnement est simple : c'est un chat dans lequel l'utilisateur peut écrire des messages et recevoir une réponse de la part d'un de nos opérateurs. C’est une page isolée, il n’y a pas besoin de navigation vers le reste de l’application.

### Outils utilisées

* HTML
* CSS / SCSS
* Javascript

### Les plus

* Responsive Design
* Mise en avant des principes BEM
* Utilisation d'un pre-processeur SCSS
* Respect des règles W3C pour optimiser le SEO : [vérifiez ici](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-inky.vercel.app%2F)
* Cross Browser : supporter sur les 2 dernières verions des navigateurs suivants à l'aide de [caniuse.com](https://caniuse.com/?compare=ie+10,ie+11,edge+87,edge+88,firefox+85,firefox+86,chrome+90,chrome+91,safari+13.1,safari+14,ios_saf+13.4-13.7,ios_saf+14.0-14.3,and_chr+88,and_ff+83&compareCats=CSS,HTML5,JS) et [autoprefixer.github.io](https://autoprefixer.github.io/) :
    - Chrome (90, 91) 
    - Firefox (85, 86) 
    - Safari (13, 14) 
    - Edge (87 / 88)
    - IE11 (90 / 91)

#### Remarque

Les src des images ne sont pas renseingées dans le HTML car elles sont chargées plus tard par le JS. Cela a posé le dilemme suivant :

⋅⋅⋅Soit je laissais les src vide et j'obtenais une erreur dans la console.

⋅⋅⋅Soit je mettais src="//:O", en designant un faux port je laissais le temps au JS de chargé les src, et je n'avais ainsi plus d'erreur dans la console. Cependant le [test](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-inky.vercel.app%2F) sur Validator W3C obtenait deux erreurs, et cela a une incidence sur le référencement. 

