# Selenium--Automation-Framework
Selenium WebDriver automation framework using Java and TestNG with basic regression test scenarios
package selenium_one1;

import java.time.Duration;

import org.openqa.selenium.By;
import org.openqa.selenium.chrome.ChromeDriver;

public class Is_Displayed {

	public static void main(String[] args) {
		ChromeDriver driver = new ChromeDriver();
        driver.manage().window().maximize();
        driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));

        driver.get("https://www.saucedemo.com/");
        boolean button= driver.findElement(By.id("login-button")).isDisplayed();
        System.out.println(button);
        driver.quit();


	}

}
