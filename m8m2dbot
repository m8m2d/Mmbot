# Mmbot
mmdbot
from selenium import webdriver
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.common.action_chains import ActionChains
import time

# Replace 'path_to_chromedriver' with the actual path to your chromedriver executable
driver = webdriver.Chrome('path_to_chromedriver')

# Replace 'your_instagram_username' and 'your_instagram_password' with your actual Instagram credentials
username = 'your_instagram_username'
password = 'your_instagram_password'

# Replace 'account_to_report' with the username of the account you want to report
account_to_report = 'account_to_report'

# Open Instagram login page
driver.get('https://www.instagram.com/accounts/login/')

# Wait for the page to load
time.sleep(2)

# Find the username and password input fields and enter your credentials
username_input = driver.find_element_by_name('username')
password_input = driver.find_element_by_name('password')
username_input.send_keys(username)
password_input.send_keys(password)

# Press Enter to log in
password_input.send_keys(Keys.ENTER)

# Wait for the page to load
time.sleep(5)

# Go to the profile page of the account you want to report
driver.get(f'https://www.instagram.com/{account_to_report}/')

# Wait for the page to load
time.sleep(2)

# Click on the three dots button to open the options menu
options_button = driver.find_element_by_css_selector('button.wpO6b')
options_button.click()

# Wait for the options menu to open
time.sleep(2)

# Find and click on the "Report" option
report_option = driver.find_element_by_xpath("//button[contains(text(), 'Report')]")
report_option.click()

# Wait for the report options to load
time.sleep(2)

# Find and click on the "It's inappropriate" option
inappropriate_option = driver.find_element_by_xpath("//button[contains(text(), 'It\'s inappropriate')]")
inappropriate_option.click()

# Wait for the confirmation dialog to load
time.sleep(2)

# Find and click on the "Report" button in the confirmation dialog
report_button = driver.find_element_by_xpath("//button[contains(text(), 'Report')]")
report_button.click()

# Wait for the report to be submitted
time.sleep(2)

# Close the browser
driver.quit()
    
