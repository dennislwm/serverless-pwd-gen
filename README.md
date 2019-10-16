# serverless-pwd-gen
Free, Fast, Secure and Serverless Password Generator

---
### About serverless-pwd-gen
This project was created by me because I couldn't find a Password generator that had these features in combination:

* Using English names or dictionary words
* Custom table mapping of alphabets to special characters
* Password strength checker
* Free, fast, responsive, secure and serverless

Basically, I'm not very good at remembering passwords. Hence, I always use English names or dictionary words as passwords. 

This becomes an issue because any potential hackers can brute hack these passwords. However, if I were to replace some alphabets with special characters, such as a -> @, then the difficulty of hacking has gone up significantly, while my password can still be easily recalled from my memory.

In other words, so long as you keep secure the custom table of maps, then you should be able to thwart hackers from guessing your passwords, while keeping your mind sane from remembering all types of weird password combinations. 

The motivation for a free, fast, secure and serverless web application came from Hat.sh, where you could encrypt a file without uploading it to a server as everything is done offline in your browser.

---
#### Responsive and Fast
Basically, I used my own [blogstrapi](https://github.com/dennislwm/blogstrapi) boilerplate as a starting point for this web app. It is responsive and fast because it uses both vanilla Bootstrap 4 and jQuery.

---
#### Secure and Serverless
As I had to find a way to generate random names, using an existing HTTP API was the easiest. However, after fetching the names, this array of strings has to be transformed using a local JSON table into possible passwords.

The **data.JSON** is a file that resides on your local computer, and it doesn't get uploaded to a server, as the post-processing is done locally in your browser.

---
![Index page](https://snipboard.io/Yvc3EJ.jpg)

---
### Prerequisites
This project is built using Bootstrap 4 and jQuery, and it has the following dependencies:
* randomuser.me - HTTP API to generate random names

As this article assumes you have some knowledge on how to build a HTML site, I will not go through the basics. 

You can always check out my article on [Creating a Blog Theme with Bootstrap and Harp](http://tldr.pro/blog/blog/creating-a-blog-theme-with-bootstrap-and-harp.html) for the basics.

---
### Project Structure
     serverless-pwd-gen/         <-- Root of your project
       |- index.html             <-- Home page of this project
       |- about.html             <-- About page of this project
       |- data.json              <-- Custom JSON table of maps
       +- css/                   <-- Holds any CSS or SCSS theme files
          |- mytheme.css         <-- Our custom CSS theme goes here

---
### Blog Article
This article [Creating a Fast, Free, Secure and Serverless Password Generator](http://tldr.pro/blog/blog/creating-a-free--fast--secure-and-serverless-password-generator.html) on my blog explains how serverless-pwd-gen was developed.

---
### Example Usage
In the following example, the default application will be created in the folder *myproject/*.

     $ git clone https://github.com/dennislwm/serverless-pwd-gen.git myproject

In the folder *myproject/*, open the file **index.html** in your web browser.

---
### Reach Out!
Please consider giving this repository a star on GitHub.

---
### License
The **serverless-pwd-gen** source code is licensed under the [GPL-3.0 license](https://github.com/dennislwm/serverless-pwd-gen/blob/master/LICENSE).