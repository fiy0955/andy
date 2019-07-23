from selenium import webdrivercl
import time


driver = webdriver.Chrome('file')
driver.get("https://accounts.google.com/signin/v2/identifier?hl=zh-TW&passive=true&continue=https%3A%2F%2Fwww.google.com%2F&flowName=GlifWebSignIn&flowEntry=ServiceLogin")
time.sleep(3)
#inp = input("輸入:")
driver.find_element_by_xpath('//*[@id="identifierId"]').send_keys("")
time.sleep(.5)
driver.find_element_by_xpath('//*[@id="identifierNext"]').click()
time.sleep(.5)
#inp = input("輸入:")
driver.find_element_by_xpath('//*[@id="password"]/div[1]/div/div[1]/input').send_keys("")
time.sleep(1)
driver.find_element_by_xpath('//*[@id="passwordNext"]').click()
driver.encoding='utf-8'
print(driver.page_source)
driver.close()
