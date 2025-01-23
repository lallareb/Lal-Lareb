# Lal-Lareb
 from PIL import Image
import requests
from io import BytesIO

# URL of the image
url = "https://raw.githubusercontent.com/lallareb/Lal-Lareb/bba5e715a63b3b83a4867ff8e04a33d891e29971/arc.jpg"

# Fetch the image from the URL
response = requests.get(url)
image = Image.open(BytesIO(response.content))

# Display the image
image.show()
