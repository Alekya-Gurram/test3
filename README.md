# test3
test3
I am editing the README file. Adding some more details about the project description.


package com.conygre.spring.boot;

import org.junit.jupiter.api.Test;
import org.springframework.boot.test.context.SpringBootTest;

@SpringBootTest
class AppConfigTest {

    @Test
    void contextLoads() {
        // Test to ensure the Spring application context loads without errors
    }
}
package com.conygre.spring.boot;

import org.junit.jupiter.api.Test;
import springfox.documentation.spring.web.plugins.Docket;

import static org.junit.jupiter.api.Assertions.*;

class SwaggerConfigTest {

    @Test
    void testNewsApiBean() {
        SwaggerConfig config = new SwaggerConfig();
        Docket docket = config.newsApi();

        assertNotNull(docket);
        assertEquals("compactdiscs", docket.getGroupName());
    }
}
