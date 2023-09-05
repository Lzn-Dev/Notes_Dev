# Les outillages utiles en dév.

## Linters

Outil qui permet d'analyser le code pour detecter les erreurs de syntaxes, problèmes de styles,
incohérences et mauvaises pratiques.
- Aide à développer et à écrire un code propre.
- Portage sur un grand nombre de langages (JS, CSS, HTML, PHP,...)
- Peuvent être intégrés dans les éditeurs de code.

Outils ->
- Php : [PhpStan](https://phpstan.org/)
- JS : [ESLint](https://eslint.org/)
- CSS : [StyleLint](https://stylelint.io/)

## Formateur de code

Outil qui permet de réorganiser automatiquement le code pour respecter les normes de codage établis.
- Aide à développer et à écrire un code propre.
- Portage sur un grand nombre de langages (JS, CSS, HTML, PHP,...)
- Peuvent être intégrés dans les éditeurs de code.

Outils -> [Prettier](https://prettier.io/).

## Documentations

Outil qui permet de générer une documentation à partir du code source.
- Portage sur un grand nombre de langages (JS, CSS, HTML, PHP,...)
- Peut générer la documentation sous différents formats (HTML, Markdown, PDF,...)

Outils ->
- JS : [JsDoc](https://jsdoc.app/)
- Php : [PhpDoc](https://www.phpdoc.org/)

## Tests
> Important de tester !

**Taux de couverture** => % du code source qui va être couvert par les tests.
*Plus il est haut -> Mieux c'est*

### Pourquoi tester ?
- Garantir la *qualité* et la *fiabilité*
- *Détecter* les erreurs avant qu'elles n'arrivent en Prod.
- Faciliter la *maintenance* et *l'évolution* du code

### Les différents types de tests
- Test unitaire
    - Test une unité de code.
    - Peut être automatisé à l'aide de frameworks de test unitaire (PhpUnit, JUnit,...)
- Test d'intégration
    - Test l'intégration de de plusieurs unités de code entre elles.
    - Peut nécessiter des environnements de tests plus complexes et simulés (BDD, APIs,...)
- Test fonctionnel
    - Test le comportement d'un systeme dans son ensemble.
    - Peut être effectuer manuellement ou automatisé à l'aide d'outils (Selenium, Cucumber,...)
- Test de performance
    - Test les perfs d'un système dans des conditions réalistes d'utilisation.
    - Peut nécessiter des outils spécifiques pour une charge élevée (JMetter, Gatling, ...)
- Test de sécurité
    - Test la sécurité d'un système.
    - Peut nécessité des outils spécialisé (OWASP ZAP, Burp Suite,...)

Outils ->
- Interfaces Web : [Playwright](https://playwright.dev/)

