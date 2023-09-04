# Sentry CheatSheet

1. Project Setting => Plateform => Choisir son framework (React, Django, ...)
2. Configurer le DSN
    1. Documentation => Chercher le framework correspondant
    2. `npm install --save @sentry/react`
    3. Suivre la configuration à integrer au code
    4. Modifier le DSN dans Sentry.init => Récuperer le DSN dans 'client keys' sur le projet Sentry
3. `npm start`
