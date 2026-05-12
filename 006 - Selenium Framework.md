* Selenium with python What is Selenium?
* What are its versions?
* Why Selenium & Advantages?
* What OS, Browsers, and Programming Languages does it Support?

**Selenium automates browsers. That's it!**

## Automation Testing
* Automated testing is a software testing technique that automates the process of validating the functionality of software without any human intervention.
* An organization can run specific software tests fastly without human testers.
* Automated testing is best suited for large or repetitive test cases.
  
## Selenium
* Selenium is an open-source, automated testing tool used to test web applications across various browsers.
* Created in the year 2004 by Jason Huggins.
* Lets us write test scripts in programming languages like Python, Ruby, Java, PHP, Perl, JavaScript, and C#.
* Selenium enables to test your website on different browsers such as Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Internet Explorer (IE).
* Automated testing with Selenium can easily scale to cover a wide range of test cases, scenarios, and user interactions.
* This scalability ensures maximum test coverage of the application’s functionality.
* Selenium supports parallel test execution, allowing multiple tests to run concurrently.

## History of Selenium
<img width="1402" height="1122" alt="image" src="https://github.com/user-attachments/assets/d9c3aea1-5cb9-4e5d-be34-779063cae19e" />


## Advantages of Selenium
1. Language and Framework Support
2. Open Source Availability
3. Multi-Browser Support
4. Support Across Various Operating Systems
5. Ease of Implementation
6. Parallel test execution
7. Easy to Learn and Use

## Disadvantages of Selenium
1. Not support for mobile and desktop applications
2. Lack of built-in reporting
3. Maintenance efforts for test scripts
4. Dependency on browser updates
5. Not Having an Image Comparison
6. Not able to automate captchas and OTP's

## Components of Selenium
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/973b038f-d4f6-4bfb-9489-3620e1edd791" />


**1. Selenium IDE**
* Selenium IDE is a Chrome and Firefox plugin.
* The primary use of a Selenium IDE is to record user interactions such as clicks, selections etc in the browser and plays them back as automated tests.
* It then generates the test script in programming languages like C#, Java, Python, and Ruby.

**Selenium IDE helps in:**
* Creating automated test scripts and validating them at speed
* Identifying and highlighting errors during the replay of interactions
* Cross Browser Testing

**2. Selenium RC**
* Selenium RC was built to automate the testing of web applications by simulating user interactions across different browsers and platforms.
* It provided a way to browser automation remotely and execute test scripts written in various programming languages.
* Not supported and deprecated.

**3. Selenium WebDriver**
* Selenium WebDriver is a powerful and enhanced version of Selenium RC which was developed to overcome the limitations of Selenium RC.
* WebDriver communicates with browsers directly with the help of browser-specific native methods.
* Test the functionality of web applications by automating user interactions such as clicking buttons, filling out forms, navigating pages, and verifying expected outcomes.
* Test web application for consistency across different browsers and browser versions (e.g., Chrome, Firefox, Edge) 

**4. Selenium Grid**
* Selenium Grid is a component of the Selenium testing framework that allows you to run test scripts across multiple browsers, operating systems, and machines in parallel.
* It enables you to perform large-scale test automation and significantly reduces the time required for testing by executing tests simultaneously on different environments.

## Selenium Versions
**Key differences between Selenium 3 and Selenium 4**
**1. WebDriver Standardization:** Selenium 4 aligns with the W3C WebDriver standard, which leads to more consistent and predictable behavior across different web browsers. This standardization reduces the compatibility issues seen in Selenium 3.

**2. Improved Selenium Grid:** Selenium 4 introduces an enhanced Grid with better support for distributed testing and improved load balancing. This makes running tests in parallel across different environments more efficient.

**3. New IDE Features:** The Selenium 4 IDE offers advanced capabilities, including improved record and playback features, support for new control flow commands, and the ability to export tests in different programming languages.

**4. Enhanced Debugging and Diagnostic Tools:** Selenium 4 provides improved logging, better screenshot capabilities, and other diagnostic tools, making it easier to troubleshoot and debug tests.

## Sample Selenium Scripts
~~~python
from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager
from time import sleep


class Suman:
   
    def __init__(self, url):
        self.url = url
        self.driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))
       
   
    def start(self):
        self.driver.get(self.url)
   
    def shutdown(self):
        self.driver.quit()


if __name__ == "__main__":
    url = "https://www.guvi.in"
    suman = Suman(url)
    suman.start()
    suman.shutdown()
~~~


