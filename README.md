from PIL import Image

# Chargement de l'image de base
base_image = Image.open("chemin/vers/image_de_base.png")

# Chargement de l'image du logo de Naruto
naruto_logo = Image.open("chemin/vers/logo_naruto.png")

# Redimensionnement de l'image du logo de Naruto pour l'adapter à la taille de l'image de base
naruto_logo = naruto_logo.resize(base_image.size)

# Combinaison des deux images
avatar_naruto = Image.blend(base_image, naruto_logo, alpha=0.5)

# Affichage de l'avatar Naruto
avatar_naruto.show()
