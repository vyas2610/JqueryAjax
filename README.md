# jQuery AJAX – Example of `$.ajax()`

This repository contains a simple and clear example of how to use **jQuery’s `$.ajax()` method** to send asynchronous HTTP requests without reloading the webpage.  
It is designed for beginners learning AJAX and how frontend interacts with backend using jQuery.

---

## 📌 Description

The **`$.ajax()`** method in jQuery is used to communicate with a server asynchronously.  
It allows web applications to:

- Send/receive data without page reload  
- Submit forms dynamically  
- Load content from API/Server in background  
- Update webpage content instantly  
- Improve user experience with smooth interactions  

This project demonstrates:

- POST request example  
- How to send data  
- How to handle success & error  
- How to show loading status  
- How AJAX connects frontend → backend  

---

## 📁 Example Code

```javascript
$.ajax({
    url: "server.php",
    type: "POST",
    data: { name: "Deepak" },
    beforeSend: function () {
        console.log("Sending request...");
    },
    success: function (response) {
        console.log("Success:", response);
    },
    error: function (xhr, status, error) {
        console.log("Error:", error);
    },
    complete: function () {
        console.log("AJAX request completed.");
    }
});
