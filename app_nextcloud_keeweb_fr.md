# L'application KeeWeb

L'application Keeweb sur le catalogue de nextcloud - [apps.nextcloud.com/keeweb](https://apps.nextcloud.com/apps/keeweb)

 - [Manipulations utiles et problèmes rencontrés](#ManipulationsUtiles)
 - [Liens utiles](#liensutiles)

L'application KeeWeb est un gestionnaire de mots de passe incorporé à Nextcloud. Elle permet par exemple de lire un fichier de type KeePass (*.kdbx*) stocké sur votre instance Nextcloud.

## Manipulations utiles & problèmes rencontrés <a name="ManipulationsUtiles"></a>
Mais il arrive parfois que Nextcloud ne laisse pas l'application prendre en charge ces fichiers, ce qui rend alors impossible leur lecture de KeeWeb. Pour remédier à cela,
[une solution](https://github.com/jhass/nextcloud-keeweb/issues/34) existe.

Se rendre dans le répertoire de configuration de Nextcloud :

```bash
cd /var/www/nextcloud/config/
```

S'il n'existe pas, créer le fichier *mimetypemapping.json* dont le propriétaire est l'utilisateur *nextcloud* :

```bash
sudo su nextcloud -c "nano mimetypemapping.json"
```

Puis ajouter dans ce fichier le texte suivent :

```bash
{
    "kdbx": ["x-application/kdbx"]
}
```

Enregistrer le fichier (**CTRL** + **o**) et quitter nano (**CTRL** + **c**).

A présent, le problème est corrigé.

## Liens utiles <a name="liensutiles"></a>
