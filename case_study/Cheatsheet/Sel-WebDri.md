# Selenium WebDriver – Bing Search

## Basic Working Steps

### 1. Import Selenium

Import the Selenium WebDriver library into your program.

```javascript
const { Builder, By, Key } = require("selenium-webdriver");
```

---

### 2. Create a Browser Driver

Tell Selenium which browser you want to automate.

**Example:**

```javascript
let driver = await new Builder()
    .forBrowser("MicrosoftEdge")
    .build();
```

This creates a connection between your program and Microsoft Edge.

---

### 3. Open a Website

```javascript
await driver.get("https://www.bing.com");
```

WebDriver opens Bing in the browser.

---

### 4. Find an Element

WebDriver finds elements on the webpage using locators.

**Example:**

```javascript
let searchBox = await driver.findElement(By.name("q"));
```

Here, Selenium finds the Bing search box using its `name` attribute.

---

### 5. Perform an Action

```javascript
await searchBox.sendKeys("Selenium WebDriver", Key.RETURN);
```

WebDriver enters the text **"Selenium WebDriver"** into the search box and presses Enter.

---

### 6. Wait / Verify

WebDriver can wait for a page or element to appear and can verify whether the expected result occurred.

For example, you can wait for search results to appear before continuing with the test.

---

### 7. Close the Browser

```javascript
await driver.quit();
```

This closes the browser and ends the WebDriver session.

---

## Complete Example

```javascript
const { Builder, By, Key } = require("selenium-webdriver");

(async function bingSearch() {
    let driver = await new Builder()
        .forBrowser("MicrosoftEdge")
        .build();

    try {
        await driver.get("https://www.bing.com");

        let searchBox = await driver.findElement(By.name("q"));

        await searchBox.sendKeys(
            "Selenium WebDriver",
            Key.RETURN
        );
    } finally {
        await driver.quit();
    }
})();
```

## Result

The Selenium WebDriver program opens Microsoft Edge, navigates to Bing, searches for **"Selenium WebDriver"**, and then closes the browser.
