# lne-doc
Pour relever le défi, nous avons decider d'exploiter une faille de sécurité. L'exploit se produit quand un site internet ajoute un lien vers le notre (`nouvelle-epoch.mff.dev`) avec l'attribut `target="_blank"`.
Lorsqu'un des visiteurs viendra cliquer sur ce lien, notre site internet se chargera correctement mais le site où le lien était présent navigera de lui même vers la page youtube du Rick Roll.
De plus, l'onglet continuera de s'actualiser toutes les 44 secondes, tant que notre site est ouvert et tant que l'autre onglet n'est pas fermé (même aprés navigation sur ce dernier). 

Pour le tester, ajouter un lien sur n'importe quel site vers le notre, comme indiqué ci dessous :

```
<a href="https://nouvelle-epoch.mff.dev" target="_blank">
```

Cette technique peut être utilisée à des fins malveillantes comme le phishing. En remplaçeant le site d'où le visiteur arrive, il est possible de voler des données personnelles/bancaires.
Beaucoup de site internet utilise encore l'attribut `target="_blank"` sans connaitre le danger que cela représente. Lorsque target="_blank" est utilisé, il est impératif de l'acompagner de l'attribut `rel="noopener noreferrer"` pour que cet exploit ne soit pas utilisable.

Cette faille peut-être exploitée en une simple ligne de javascript:

```javascript
window.opener.location.href = "https://lien-malveillant.com"
```

window.opener fait référence à l'onglet du lien et changer le location.href de window.opener cause une navigation sur cet onglet.
