from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager

# Start Chrome
driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))

# Open Google
driver.get("https://www.whatsapp.com/")

input("Press Enter to close...")

driver.quit() 
#pip install webdriver-manager

from selenium import webdriver
from selenium.webdriver.common.by import By

# Start Chrome browser
driver = webdriver.Chrome()

# Open Google homepage
driver.get("https://www.google.com/")

# Inspect and locate search box element
search_box = driver.find_element(By.NAME, "q")

# Print confirmation
print("Search box element found:", search_box)

# Keep browser open until user input
input("Press Enter to close...")

# Close browser
driver.quit()
