

# Remove Background

from rembg import remove // import libary rembg
from PIL import Image

input_path = 'buah.jpg' //pengen file gambar 
output_path = 'newBuah.png' //export to png

input_image = Image.open(input_path)
output_image = remove(input_image)
output_image.save(output_path) // save file pada folder default

// show image after and before remove

import matplotlib.pyplot as plt //libary plotlib 

input_path = 'buah.jpg'
output_path = 'newBuah.png'

# Buka gambar asli
input_image = Image.open(input_path)

# Tampilkan gambar asli sebelum penghapusan latar belakang
plt.subplot(1, 2, 1)
plt.imshow(input_image)
plt.title('Original Image')

# Hapus latar belakang
output_image = remove(input_image)

# Tampilkan gambar setelah penghapusan latar belakang
plt.subplot(1, 2, 2)
plt.imshow(output_image)
plt.title('Image with Removed Background')

# Simpan gambar yang telah dihapus latar belakang
output_image.save(output_path)

# Tampilkan plot
plt.tight_layout()
plt.show()

// hasil output





## Screenshots


!![Image](readme_images/.png)(https://via.placeholder.com/468x300?text=App+Screenshot+Here)



## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## screen shoot
![Image](UAS-PA-PC-FittoMartcellindo-202131001-Ss-HAsil-sourcecode.png)
