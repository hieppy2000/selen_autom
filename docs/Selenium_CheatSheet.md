# Get parent of webelement:
- parent_elem = driver.execute_script("return arguments[0].parentNode;", elem)

# BODY of the page element:
- driver.find_element_by_css_selector("BODY")
