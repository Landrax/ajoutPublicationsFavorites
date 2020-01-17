<a href="www.etvoilacamarche.fr"><img src="https://etvoilacamarche.fr/wp-content/uploads/2018/10/LogoEtVoilaCaMarche-Noir-v3.0-2.svg" title="Et Voila Ca Marche" alt="Et voila ca marche"></a>

***Exercice de mise en ligne d'un projet AJAX via Git***


# AJOUT D'ARTCILES FAVORIS
> Des articles apparaissent pour l'utilisateur. Au clic, l'article est ajouté aux favoris via la SESSION, lors du déclic, l'icone favoris disparait et l'article est enlevé de la SESSION.

> Tech: AJAX, Javascript, PHP

**N'oubliez pas ...**
- Si vous souhaitez lier à une base de données, créer votre fichier d'initialisation dans le dossier inc.
- Les articles apparaissent en "dur"  dans notre index, veuillez les remplacer par les vôtres.

> Ajout de notre GIF [![LES FAVORIS  SELON MOI](https://media.giphy.com/media/GHcm2aWIczatG/giphy.gif)]()

## Table des matières

- [Explication](#explication)
- [Remerciements](#remerciements)

---
## Explication
---

```PHP
// Retrait des favoris en SESSION
   if(isset($_POST["a"]) && $_POST["a"] == "remove")
            {
                foreach ($_SESSION['favorites'] as $key => $value)
                {
                  if($id == $value)
                  {
                    unset($_SESSION['favorites'][$key]);
                  }
                }
            }

            print "true";
        } else {
            print "false";
        }



```
- Pour retirer les favoris de ma SESSION, je regarde bien que l'action demandée est un "remove"
- Je fais concoreder le $id envoyé en POST avec les valeurs enregistrées en SESSION
---
## Remerciements
---

A tous les étudiants !

[![Veuillez visiter notre site](https://media.giphy.com/media/3o6EhGvKschtbrRjX2/giphy.gif)](https://www.keepizi.com)