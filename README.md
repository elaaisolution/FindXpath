# FindXpathwrapper

Selenium Xpath wrapper , support browsers Chrome, Firefox, Supported OS Windows, Linux, Ubuntu, Mac

# Xpath Wrapper
------------
    Selenium xpath wrapper framework
# Examples :

# To Use Chrome Browser :

### from xpathwrapper.basec import driver,checkbyxpath

### driver.get('http://testing.pythonautomation.tk/')

### checkbyxpath("//ul[@class='actions']//li/a[text()='Test Me']").click()

# To Use Firefox Browser :

### from xpathwrapper.basec import driver,checkbyxpath

### driver.get('http://testing.pythonautomation.tk/')

### checkbyxpath("//ul[@class='actions']//li/a[text()='Test Me']").click(
.................................... Key Words ..........................

# checkbyid(locator):
    """
    checkbyid(locator)

    Locating by Id; Use this when you know id attribute of an element. With this strategy, 
    the first element with the id attribute value matching the location will be returned.
    If no element has a matching id attribute, a NoSuchElementException will be raised..
     
    checkbyid('loginForm')
    
    """
    driver.find_element_by_id(locator)
    
# checkbyname(locator):
    """
    checkbyname(locator)

    Locating by Name; Use this when you know name attribute of an element. With this strategy,
     the first element with the name attribute value matching the location will be returned. 
     If no element has a matching name attribute, a NoSuchElementException will be raised. 
    
    checkbyname('username')
    
    """
    driver.find_element_by_name(locator)

# checkbyxpath(locator):
    """
    checkbyxpath(locator)

    Locating by XPath; XPath is the language used for locating nodes in an XML document. As HTML can 
    be an implementation of XML (XHTML), Selenium users can leverage this powerful language to target 
    elements in their web applications. XPath extends beyond (as well as supporting) the simple methods 
    of locating by id or name attributes, and opens up all sorts of new possibilities such as locating 
    the third checkbox on the page.

    One of the main reasons for using XPath is when you don't have a suitable id or name attribute for 
    the element you wish to locate. You can use XPath to either locate the element in absolute terms 
    (not advised), or relative to an element that does have an id or name attribute. XPath locators can 
    also be used to specify elements via attributes other than id and name.

    Absolute XPaths contain the location of all elements from the root (html) and as a result are likely 
    to fail with only the slightest adjustment to the application. By finding a nearby element with an id 
    or name attribute (ideally a parent element) you can locate your target element based on the 
    relationship. This is much less likely to change and can make your tests more robust. 
    
    checkbyxpath('/html/body/form[1]')
    
    """
    driver.find_element_by_xpath(locator)

# checkbylinktext(locator):
    """
    checkbylinktext(locator)

    Locating Hyperlinks by Link Text; Use this when you know link text used within an anchor tag. 
    With this strategy, the first element with the link text value matching the location will be 
    returned. If no element has a matching link text attribute, a NoSuchElementException will be raised.

    checkbylinktext('Continue')
    
    """
    driver.find_element_by_link_text(locator)
    
# checkbypartialtext(locator):
    """
    checkbypartialtext(locator)

    findFileByName; Search the file by using name of the file in directory.
    Once using name indicates the file name and path indicates the directory where
    you want to search. 
    
    checkbypartialtext('Conti')
    
    """
    driver.find_element_by_partial_link_text(locator)

# checkbytag(locator):
    """
    checkbytag(locator)

    Locating Elements by Tag Name; Use this when you want to locate an element by tag name. 
    With this strategy, the first element with the given tag name will be returned. If no 
    element has a matching tag name, a NoSuchElementException will be raised.
    
    checkbytag('h1')
    
    """
    driver.find_element_by_tag_name(locator)
    
# checkbyclass(locator):
    """
    checkbyclass(locator)

    Locating Elements by Class Name; Use this when you want to locate an element by class 
    attribute name. With this strategy, the first element with the matching class attribute 
    name will be returned. If no element has a matching class attribute name, a 
    NoSuchElementException will be raised. 
    
    checkbyclass('content')
    
    """
    driver.find_element_by_class_name(locator)
    
# checkbycss(locator):
    """
    checkbycss(locator)

    Locating Elements by CSS Selectors; Use this when you want to locate an element by CSS selector
    syntax. With this strategy, the first element with the matching CSS selector will be returned.
    If no element has a matching CSS selector, a NoSuchElementException will be raised. 
    
    checkbycss('p.content')
    
    """
    driver.find_element_by_css_selector(locator)

# checkbynames(locator):
    """
    checkbynames(locator)

    Locating by Name; Use this when you know name attribute of an element. With this strategy,
    the first element with the name attribute value matching the location will be returned. 
    If no element has a matching name attribute, a NoSuchElementException will be raised. 
    
    checkbynames('username')
    
    """
    driver.find_elements_by_name(locator)
  
# checkxpathelements(locator):
    """
    checkxpathelements(locator)

    Locating by XPath; XPath is the language used for locating nodes in an XML document. As HTML can 
    be an implementation of XML (XHTML), Selenium users can leverage this powerful language to target 
    elements in their web applications. XPath extends beyond (as well as supporting) the simple methods 
    of locating by id or name attributes, and opens up all sorts of new possibilities such as locating 
    the third checkbox on the page.

    One of the main reasons for using XPath is when you don't have a suitable id or name attribute for 
    the element you wish to locate. You can use XPath to either locate the element in absolute terms 
    (not advised), or relative to an element that does have an id or name attribute. XPath locators can 
    also be used to specify elements via attributes other than id and name.

    Absolute XPaths contain the location of all elements from the root (html) and as a result are likely 
    to fail with only the slightest adjustment to the application. By finding a nearby element with an id 
    or name attribute (ideally a parent element) you can locate your target element based on the 
    relationship. This is much less likely to change and can make your tests more robust. 
    
    checkxpathelements('/html/body/form[1]')
    
    """
    driver.find_elements_by_xpath(locator)

# checkbylinktexts(locator):
    """
    checkbylinktexts(locator)

    Locating Hyperlinks by Link Text; Use this when you know link text used within an anchor tag. 
    With this strategy, the first element with the link text value matching the location will be 
    returned. If no element has a matching link text attribute, a NoSuchElementException will be raised.

    checkbylinktexts('Continue')
    
    """
    driver.find_elements_by_link_text(locator)
    
# checkbypartialtexts(locator):
    """
    checkbypartialtexts(locator)

    findFileByName; Search the file by using name of the file in directory.
    Once using name indicates the file name and path indicates the directory where
    you want to search. 
    
    checkbypartialtexts('Conti')
    
    """
    driver.find_elements_by_partial_link_text(locator)

# checkbytagelements(locator):
    """
    checkbytagelements(locator)

    Locating Elements by Tag Name; Use this when you want to locate an element by tag name. 
    With this strategy, the first element with the given tag name will be returned. If no 
    element has a matching tag name, a NoSuchElementException will be raised.
    
    checkbytagelements('h1')
    
    """
    driver.find_elements_by_tag_name(locator)
 
# checkbyclassnames(locator):
    """
    checkbyclassnames(locator)

    Locating Elements by Class Name; Use this when you want to locate an element by class 
    attribute name. With this strategy, the first element with the matching class attribute 
    name will be returned. If no element has a matching class attribute name, a 
    NoSuchElementException will be raised. 
    
    checkbyclassnames('content')
    
    """
    driver.find_elements_by_class_name(locator)
    
# checkbycssselectors(locator):
    """
    checkbycssselectors(locator)

    Locating Elements by CSS Selectors; Use this when you want to locate an element by CSS selector
    syntax. With this strategy, the first element with the matching CSS selector will be returned.
    If no element has a matching CSS selector, a NoSuchElementException will be raised. 
    
    checkbycssselectors('p.content')
    
    """
    driver.find_elements_by_css_selector(locator)
