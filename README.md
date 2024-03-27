# 123123


from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time

driver = webdriver.Chrome()
driver.maximize_window()
driver.get("https://calcus.ru/kalkulyator-ipoteki")
elem = driver.find_element(By.NAME,"cost")
elem.click()
elem.send_keys("111111")
elem = driver.find_element(By.NAME,"start_sum")
elem.clear()
elem.send_keys("22222")
elem = driver.find_element(By.NAME,"period")
elem.clear()
elem.send_keys("30")
elem = driver.find_element(By.NAME,"percent")
elem.clear()
elem.send_keys("15")
elem.send_keys(Keys.ENTER)

time.sleep(5)
