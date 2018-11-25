# webpage
open urls in a specific browser

## Usage
```webpage``` expects the location of an executable of the brower to be passed. As long
as the browser supports command line interfaces ```webpage``` will work.

## Examples

### using Firefox
```
from webpage import webpage

firefox_executable_path = r'C:\Program Files\Mozilla Firefox\firefox.exe'
browser = webpage(firefox_executable_path)

urls_to_open = ['https://google.com', 'https://amazon.com', 'https://instagram.com']
for url in urls_to_open:
  browser.open(url)
```


### using Google Chrome

```
from webpage import webpage

chrome_executable_path = r"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe"
browser = webpage(chrome_executable_path)

browser.open('https://youtube.com')
```
