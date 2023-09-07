FONCTIONNEMENT :
- Pour pouvoir joindre les cgv, celles-ci doivent êtres placées dans les documents de Dolibarr dans mycompany/cgv/ sous le nom de cgv.pdf
  Si vous utilisez le module multicompany, ce sera sous x/mycompany/cgv/ où x est la référence de l'entité.
  Pour mettre en place des cgv internationales, il suffit de créer un dossier pour le pays (exemple : en_US pour l'anglais)
- Pour mettre un logo spécifique dans RUBIS (devis), il suffit de mettre en place la constante RUBIS_LOGO_RUBIS avec pour valeur le nom du fichier image. L'image doit être présente dans documents/mycompany/logos
- Pour mettre un logo spécifique dans EDISON (commande), il suffit de mettre en place la constante RUBIS_LOGO_EDISON avec pour valeur le nom du fichier image. L'image doit être présente dans documents/mycompany/logos
- Pour mettre un logo spécifique dans HOMARD (facture), il suffit de mettre en place la constante RUBIS_LOGO_HOMARD avec pour valeur le nom du fichier image. L'image doit être présente dans documents/mycompany/logos
- Pour mentionner le montant d'un acompte sur RUBIS, il suffit de créer un attribut supplémentaire sur les propale de type décimal, code "deposit", libéllé au choix. Le pourcentage est à saisir dans la propale.

Pour activer les options, il faut créer les constantes suivantes dans Accueil => Configuration => Divers
   RUBIS_SIGNATURE_AREA avec la valeur à 1 = Affiche la signature RUBIS
   RUBIS_SIGNATURE_AREA avec la valeur à 0 = Pas de zone de signature
   RUBIS_SIGNATURE_AREA n'existe pas = signature native de Dolibarr
   RUBIS_FOLD_MARK avec valeur à 1 = impression du repère de pliage
   
   RUBIS_LOGO_RUBIS avec le nom de l'image à utiliser pour le devis
   RUBIS_LOGO_EDISON avec le nom de l'image à utiliser pour la commande
   RUBIS_LOGO_HOMARD avec le nom de l'image à utiliser pour la facture
