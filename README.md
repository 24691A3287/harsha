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
driver = webdriver.Chrome()
driver.get("https://www.google.com/")
search_box = driver.find_element(By.NAME, "q")
print("Search box element found:", search_box)
input("Press Enter to close...")
driver.quit()
