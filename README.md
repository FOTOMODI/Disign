# Disign
Disign foto
from PIL import Image, ImageFilter

# Open an image file
image_path = 'path/to/your/image.jpg'
original_image = Image.open(image_path)

# Display the original image
original_image.show()

# Convert the image to grayscale
gray_image = original_image.convert('L')

# Display the grayscale image
gray_image.show()

# Apply a blur filter to the original image
blurred_image = original_image.filter(ImageFilter.BLUR)

# Display the blurred image
blurred_image.show()

# Save the processed images
gray_image.save('path/to/your/gray_image.jpg')
blurred_image.save('path/to/your/blurred_image.jpg')
