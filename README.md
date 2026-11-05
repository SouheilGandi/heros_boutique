 objets = {
    "épée": 10,
    "bouclier": 8,
    "potion": 5,
    "arc": 12,
    "casque": 7,
    "armure": 15,
    "carte": *,      # indice : la carte coûte 2 pièces
    "clé": *         # indice : la clé coûte 3 pièces
}
 
argent = 20
sac = **             # une liste vide : le sac du héros
 
****("⚔️ Bienvenue dans la Boutique du Héros !")
print("Tu as", argent, "pièces.")
print("Écris le nom d'un objet pour l'acheter.")
print("Écris 'boutique' pour voir les objets, 'sac' pour ouvrir ton sac, 'quitter' pour partir.")
 
while ****:
    choix = *****("\nQue veux-tu faire ? ").lower().*****()
 
    # ----- Voir la boutique -----
    if choix == "boutique":
        print("--- BOUTIQUE ---")
        print("épée : 10 pièces")
        print("bouclier : 8 pièces")
        print("potion : 5 pièces")
        print("arc : 12 pièces")
        print("casque : 7 pièces")
        print("armure : 15 pièces")
        print("carte : 2 pièces")
        print("clé : 3 pièces")
 
    # ----- Ouvrir le sac -----
    elif choix == "sac":
        if len(sac) == *:
            print("Ton sac est vide.")
        else:
            print("Dans ton sac :")
            for objet ** sac:
                print("-", ******)
 
    # ----- Quitter -----
    elif choix == "quitter":
        print("Bonne aventure, héros !")
        *****
 
    # ----- Acheter un objet -----
    elif choix in ******:
        prix = objets[******]
 
        if argent >= ****:
            argent = argent - ****
            sac.******(choix)
            print("Tu as acheté :", choix, "! Il te reste", argent, "pièces.")
        ****:
            print("Pas assez de pièces...")
 
    # ----- Objet inconnu -----
    else:
        print("Cet objet n'existe pas.")
 
print("\n--- FIN DE L'AVENTURE ---")
print("Pièces restantes :", ******)
print("Objets dans ton sac :", len(***))
 
if len(sac) >= 3:
    print("🛡️ Tu es bien équipé !")
****:
    print("⚠️ Tu n'es pas assez équipé pour affronter le dragon...")
 
Claude finished the response
