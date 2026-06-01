Import requests
from bs4 import BeautifulSoup

# Website link
url = "https://example.com"

# Request page data
response = requests.get(url)

# Parse HTML
soup = BeautifulSoup(response.text, "html.parser")

# Title print
print("Page Title:")
print(soup.title.text)

