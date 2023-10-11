**Title**

Selection of Backend Language 

**Status**

Accepted

**Context**

The backend language plays a crucial role in the mobile app in managing and facilitating various important requirements that the app provides, such as ride booking, real-life tracking, user data handling, and secure payment. It needs to handle a high number of real-time data processing as well as transactions under heavy usage such as peak hours. As mentioned in the requirements, the backend language must be compatible with geolocation services since the app requires their integration. For the payment transactions to be managed securely and with reliability, the backend language should integrate with the payment gateway APIs effectively. Therefore, the decision to select a suitable backend language is pivotal in terms of functions, performance, and security as the app continues to develop and grow.

**Decision**

Node.js is implemented as the backend language, primarily due to its performance in handling asynchronous operations and real-time applications, which are critical to the requirements of the mobile app. As there will be numerous events happening at once, like ride booking and payment processing, Node.js will be able to handle multiple requests simultaneously without affecting its speed or performance. Although Python (Django/Flask) is a versatile language, it generally performs not as efficiently as Node.js when it comes to handling multiple real-time connections and asynchronous I/O operations. PHP, despite its wide usage in web development, similarly does not perform as well as Node.js in real-time applications and can experience limitations in handling non-blocking I/O operations.

In addition, Node.js can incorporate geolocation services using various libraries and APIs such as Google Maps Geolocation API. Furthermore, the node package manager (NPM) library provides a wide variety of support and information from different developers, which can facilitate the development process of the app. Java (Spring) meanwhile is more resource-intensive and might require more coding in the process, which might slow down the development process.

**Consequences**

By deploying Node.js, heavy numbers of events and tasks can be managed and maintained at the same time, allowing the app to run smoothly despite its heavy usage, and ensuring a positive user experience. As the app might continue to develop more functions and features under increasing usage, Node.js will be capable of handling this due to its nature.

However, even though Node.js is widely used and has a big community with a wide range of available tools, it is critical that the tools, packages, libraries, and resources chosen are reliable and will continue to be supported in the future. By doing so, the app can be maintained effectively without any potential disruptions or redevelopment work.
