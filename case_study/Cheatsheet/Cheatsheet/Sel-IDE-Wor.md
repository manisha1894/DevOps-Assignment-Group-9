# Selenium IDE – Web Automation Cheat Sheet

## Objective

To perform basic web automation testing using **Selenium IDE** by recording and executing a test case for a search operation.

---

## Requirements

* Windows/Linux/macOS
* Google Chrome or Microsoft Edge
* Selenium IDE browser extension
* Internet connection

---

## 1. Install Selenium IDE

1. Open Google Chrome or Microsoft Edge.
2. Go to the browser's extension store.
3. Search for **Selenium IDE**.
4. Install the Selenium IDE extension.
5. Open Selenium IDE from the browser extensions.

---

## 2. Create a New Project

1. Open Selenium IDE.
2. Select **Create a new project**.
3. Enter the project name:

```text
Search Automation Test
```

4. Enter the Base URL:

```text
https://www.bing.com
```

5. Click **OK/Create**.

---

## 3. Create a Test Case

Create a new test case with the name:

```text
Bing Search Test
```

The test case will automate a search operation on Bing.

---

## 4. Record the Test

1. Open the Selenium IDE project.
2. Select **Record a new test**.
3. Open the Bing website.
4. Click on the search box.
5. Enter:

```text
Selenium WebDriver
```

6. Click the **Search** button.
7. Stop the recording.

Selenium IDE automatically records the actions performed on the webpage.

---

## 5. Recorded Test Steps

The recorded test may contain commands similar to:

| Command       | Target        | Value              |
| ------------- | ------------- | ------------------ |
| `open`        | `/`           |                    |
| `click`       | Search box    |                    |
| `type`        | Search box    | Selenium WebDriver |
| `click`       | Search button |                    |
| `assertTitle` | Page title    |                    |

> The exact target values may differ depending on the browser and webpage version.

---

## 6. Important Selenium IDE Commands

### Open

Used to open a webpage or URL.

```text
Command: open
Target: /
```

### Click

Used to click an element.

```text
Command: click
Target: <element>
```

### Type

Used to enter text into an input field.

```text
Command: type
Target: <search box>
Value: Selenium WebDriver
```

### Wait For Element Visible

Waits until a particular element becomes visible.

```text
Command: wait for element visible
Target: <element>
```

### Assert Text

Checks whether specific text exists on the webpage.

```text
Command: assert text
Target: <element>
Value: Selenium WebDriver
```

### Assert Title

Checks the title of the webpage.

```text
Command: assert title
Target: <page title>
```

---

## 7. Run the Test

1. Open the **Bing Search Test** test case.
2. Click the **Run current test** button.
3. Selenium IDE executes the recorded commands automatically.
4. Observe the browser while the test is running.
5. Check the test result shown in Selenium IDE.

---

## 8. Expected Result

The test should:

1. Open Bing.
2. Locate the search box.
3. Enter **Selenium WebDriver**.
4. Perform the search.
5. Display search results related to Selenium WebDriver.
6. Complete the test successfully.

---

## 9. Example Test Flow

```text
Start
  ↓
Open Bing
  ↓
Click Search Box
  ↓
Enter "Selenium WebDriver"
  ↓
Click Search
  ↓
Verify Search Results
  ↓
Test Passed
```

---

## 10. Common Errors

### Element Not Found

**Problem:** Selenium IDE cannot locate an element.

**Solution:**

* Check the target locator.
* Re-record the step.
* Make sure the webpage has loaded completely.

### Page Not Loading

**Problem:** The website does not open.

**Solution:**

* Check your internet connection.
* Verify the Base URL.
* Try opening the website manually.

### Test Failed

**Problem:** One or more commands fail.

**Solution:**

* Check the failed command.
* Verify the target and value.
* Run the test again.

---

## 11. Advantages of Selenium IDE

* Easy to install and use.
* No programming knowledge is required for basic recording.
* Automatically records browser actions.
* Useful for creating quick automated test cases.
* Supports playback of recorded tests.
* Helps beginners understand web automation.

---

## 12. Result

The **Bing Search Test** was successfully created and executed using **Selenium IDE**. The test automated the process of opening Bing, entering a search query, performing the search, and verifying the result.

---

## Conclusion

Selenium IDE provides a simple way to automate web application testing by recording user actions and replaying them as automated test cases. It is useful for beginners to understand the basic concepts of browser automation and software testing.
