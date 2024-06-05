from PIL import Image
import pytesseract

# Ruta a la imagen
image_path = r"C:\Users\MINEDUCYT\Desktop\48bc80e9-cc72-4695-9c92-c31ccf7a2d9d.jpg"

# Abrir imagen
image = Image.open(image_path)

# Usar pytesseract para extraer texto
extracted_text = pytesseract.image_to_string(image, lang='spa')

# Mostrar el texto extraído
print(extracted_text)
