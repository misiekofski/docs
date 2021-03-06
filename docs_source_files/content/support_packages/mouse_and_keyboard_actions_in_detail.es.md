---
title: "Acciones en detalle del mouse y teclado"
weight: 4
---

{{% notice info %}}
<i class="fas fa-language"></i> Page being translated from 
English to Spanish. Do you speak Spanish? Help us to translate
it by sending us pull requests!
{{% /notice %}}


Suppose you have an arbitrary web element **e:**

{{< code-tab >}}
  {{< code-panel language="java" >}}
WebElement e = driver.findElement(By.id("testElement"));
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
e = driver.find_element_by_id("testElement")
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}

You can simulate mouse clicking on e if it's visible and has a height and width
that are greater than 0:

{{< code-tab >}}
  {{< code-panel language="java" >}}
e.click();
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
e.click()
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}

Moreover, it's possible to mimic hovering of the cursor over **e**. In order
to do so, you'll need the following import statement:

{{< code-tab >}}
  {{< code-panel language="java" >}}
import org.openqa.selenium.interactions.Actions;
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
from selenium.webdriver import ActionChains
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}

With this statement in place, you can now move over the element in question:

{{< code-tab >}}
  {{< code-panel language="java" >}}
Actions actions = new Actions(driver);
actions.moveToElement(e);
actions.perform();
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
actions = ActionChains(driver)
actions.move_to_element(e)
actions.perform()
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}

If **e** is an **input** or **textarea** element, the following keyboard 
actions can be carried out:

1. Enter a sequence of characters in e:

{{< code-tab >}}
  {{< code-panel language="java" >}}
e.sendKeys("Test");
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
e.send_keys("Test")
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}

<p>2. Delete the text that's in e (if there is any):

{{< code-tab >}}
  {{< code-panel language="java" >}}
e.clear();
  {{< / code-panel >}}
  {{< code-panel language="python" >}}
e.clear()
  {{< / code-panel >}}
  {{< code-panel language="csharp" >}}
// We don't have a C# code sample yet -  Help us out and raise a PR
  {{< / code-panel >}}
  {{< code-panel language="ruby" >}}
# We don't have a Ruby code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
  {{< code-panel language="javascript" >}}
// We don't have a JavaScript code sample yet -  Help us out and raise a PR  
  {{< / code-panel >}}
{{< / code-tab >}}