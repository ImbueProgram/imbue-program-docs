
# Introduction:

Try to think of apps as web pages. They have sections, buttons, texts, etc. and you can interact with them through your [browser](https://en.wikipedia.org/wiki/Web_browser) (in your phone, computer, tv, etc.).

Applications are made of files. Like a MS Word document (.doc), or a MS Excel spreadsheet (.xls) or a song (.mp3), a web is made of one or more files, and you need a program to open them like you need MS Word to open a word document.

So basically, to simplify a lot, a website is like a Word document, but usually located in a place where people can have access to it through Internet. We will speak about this place in further lessons.

Another difference, is that you need MS Word for both, editing and opening a word file, but in our case, for the files we will work with, you will only need a text editor to write your code, and a browser to run it.

## Applications and Internet


Internet plays a very important role when speaking about web applications, as everything works through a network, you need to deal with problems like:

- Access control to documents (Security)
- Bandwidth limitations (Speed)

As you know, networks (Internet) sometimes are slow, and sometimes you need to access to some private information which is stored remotely (like your email).

That's why we don't store all the information in the same public document, because it could be very large and because it might not be safe to expose some information to anyone.

For this same purpose, websites usually retrieve some of their data (like a list of movies in filmaffinity.com) from an external source, such as, a database, RSS, or any other. So they can show you a different list of movies based on your user, or on your location without needing to have all the variations loaded at once.

![Internet apps](https://cognos.com.bo/wp-content/uploads/2019/05/bannerwebapplication-1.jpg)

For example, [Shazam](https://www.shazam.com/) lets you find a song that is playing just hearing it a pair of seconds. To do that, shazam would need some sort of database, and a way of contrasting your sound with that database. Then, respond with a match.
Obviously, Shazam does not load that database in your phone, instead, you send a small package with your audio, it searches on its databases and responds the best match. The programs in charge of that comparison and search, are considered backend.

## Servers and clients

To create any kind of network, you need servers and clients. A [server](<https://en.wikipedia.org/wiki/Server_(computing)>) is a program that makes information available when its requested from some a source (like a browser), a [client](<https://en.wikipedia.org/wiki/Client_(computing)>) is a program that requests the information, and will be ready to receive it and display it.

There are different kind of clients, and different kind of servers. Is not the same a server that serves websites than a server that serves music or torrents, or a database. And its not the same a client that requests websites, than one requesting p2p files (torrent)

You will learn more about these concepts in future lessons.

## Frontend, backend, devops, fullstack:

When building applications, you need to solve different stages for your app to be available for everyone, like:

- Doing layouts in HTML and CSS
- Adding logic and behavior to your designs with Javascript
- Doing tests
- Making everything online on the web

### [Frontend](https://en.wikipedia.org/wiki/Front_and_back_ends)

Usually refers to the part of the application that is executed inside the browser (client).

### [Backend](https://en.wikipedia.org/wiki/Front_and_back_ends)

Refers to the part of the appilcation that is executed outside the client, in any other service running in a different server.

### [DevOps](https://en.wikipedia.org/wiki/DevOps)

Usually referred to the part of making our programs available through networks, scaling them and serving them. They are the masters of servers.

### Fullstack

Refers to the complete pack.

## Javascript
![Javascript](https://i0.wp.com/www.vidagnu.com/wp-content/uploads/2014/12/javascript.png?fit=800%2C300&ssl=1)

This is the main language we will teach you here. We will show you how it looks like, don't worry if you don't understand anything for the moment:

```javascript
console.log("Hello world!");
```

### Javascript is NOT Java

Java and Javascript mostly have the name in common, but they are different languages made for different purposes. This is how the same program would be written in Java instead:
```java
System.out.println("Hello, World");
```

Javascript is a client / server based language while java needs a virtual machine to run and its mostly used for backend.