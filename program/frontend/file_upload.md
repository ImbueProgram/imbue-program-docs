# Files Upload

Understanding file upload.

## What are files?
A file is an object on a computer that stores data, information, settings. In the browser you will usually work with Images, Videos, Documents, compressed files and audio.

## How are files transfered?
To transfer a file from a web browser to an API the whole binary data of a file needs to be sended. 
The way to perform a file upload in the browser is to use [XMLHttpRequest](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest).

## Different ways of uploading a file
- Using the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). Fetch API is am interface to XMLHttpRequest, with a more powerful and flexible feature set.
- [Sending a form](https://developer.mozilla.org/en-US/docs/Web/API/FormData/Using_FormData_Objects#Retrieving_a_FormData_object_from_an_HTML_form). `request.send(new FormData(input.form))`. Here the form contents will be encoded as `multipart/form-data`, meaning that you can send multiple form fields and metadata like field and file names will be transmitted as well. You can also [modify the FormData object](https://developer.mozilla.org/en-US/docs/Web/API/FormData#Methods) before sending it. Depending on the server-side framework, handling this request might be simpler than raw data, there are typically many helpers you can use

## Receiving files in the server side
TODO

## Progress

You can listen to [progress events on XMLHttpRequest.upload.](https://developer.mozilla.org/en-US/docs/Using_files_from_web_applications#Handling_the_upload_process_for_a_file) The [progress events](https://developer.mozilla.org/en-US/docs/Web/API/ProgressEvent) have `loaded` and `total` properties that allow determining how far you've got with your request.

## Keep the user informed:
Information about the file that can be made available to the user:

- File Name
- File Size
- Mime Type
- A Progress bar with percent complete
- The upload speed or upload bandwidth
- The approximate time remaining
- The bytes uploaded thus far
- A response from the server side

## Tutorials
- [A strategy for multiple file uploads in JavaScript](https://medium.com/typecode/a-strategy-for-handling-multiple-file-uploads-using-javascript-eb00a77e15f)
- [Handling files in Node](http://howtonode.org/really-simple-file-uploads)

# Exercise: Making a file upload 

This exercise called 'File Upload' consists on the following requirements:
- Create a website where users can drag & drop multiple files and submit them.
    - Hint: You can use [Dropzone](https://www.dropzonejs.com/)
- Create an API that handles the files requests and stores them.
- Show the uploaded files in your website and allow to delete them.

