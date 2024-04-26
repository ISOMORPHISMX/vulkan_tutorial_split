

```plantuml
class GlobalVariable {
    const uint32_t WIDTH = 800
    const uint32_t HEIGHT = 600
}

class HelloTriangleApplication {
    -GLFWwindow* window
    -VkInstance instance
    +run()
    -initWindow()
    -initVulkan()
    -mainLoop()
    -cleanUp()
    -createInstance()
}

class main {
    HelloTriangleApplication app
    app.run()
}
GlobalVariable<--HelloTriangleApplication
HelloTriangleApplication<--main
```




