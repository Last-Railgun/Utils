package com.demo.util;

import org.jetbrains.annotations.NotNull;
import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

/**
 * SpringUtils
 *
 * @author Syz
 * @version 1.0
 */
public class SpringUtils {
    private static ApplicationContext context;
    static {
        context = new ClassPathXmlApplicationContext("applicationContext.xml");
    }
    /**
     * Obtain the corresponding bean according to the bean name
     * in the spring container or the value defined by the 
     * ID attribute in the configuration file < bean >
     *
     * @param beanName The bean name or ID attribute to get
     * @param <T> In order to adapt to different types of beans, generics are used as placeholders
     * @return Returned bean (note the returned type)
     */
    @NotNull
    public static <T> T getBean(String beanName) { return (T) context.getBean(beanName); }
}
