# FileSystem over Cookies in JS

## Table of Contents
- Introduction
- Installation
- Usage
- Example Usage
- Important Notes
- Further Resources
- Contributing
- License

## Introduction

The `FileSystem` JavaScript class simulates a basic file system within a web browser environment. It allows you to create, manipulate, and delete directories and files, utilizing cookies for persistence. This makes it suitable for experimenting with file system-like operations in a controlled and accessible manner, especially for educational purposes.

## Installation

While this class doesn't require any specific installation procedures, a basic understanding of JavaScript and its interaction with web browsers is necessary for effective utilization within your projects.

## Usage

### Import the Class:

```javascript
import FileSystem from './FileSystem.js'; // Adjust the path if necessary
```
Available Methods:
- createDirectory(path): Creates a new directory at the specified path.
- createFile(path, content): Creates a file at the specified path, containing the provided content.
- readDirectory(path): Returns an array of filenames or subdirectory names within the directory at the given path.
- readFile(path): Returns the content of the file at the specified path.
- deleteEntry(path): Deletes the directory or file at the provided path.

### Example Usage
``` javascript
// Create directories
fileSystem.createDirectory('/root');
fileSystem.createDirectory('/root/documents');
```
``` javascript
// Create a file
fileSystem.createFile('/root/documents/file1.txt', 'This is the content of file1.txt');
```
``` javascript
// Read directory contents
const directoryContents = fileSystem.readDirectory('/root/documents');
console.log(directoryContents); // Output: ['file1.txt']
```
``` javascript
// Read file content
const fileContent = fileSystem.readFile('/root/documents/file1.txt');
console.log(fileContent); // Output: 'This is the content of file1.txt'
```
``` javascript
// Delete a file
fileSystem.deleteEntry('/root/documents/file1.txt');
```
### Important Notes
This class is primarily intended as a demonstrative tool for educational purposes and is not recommended for production environments. For robust file system functionalities in production settings, consider utilizing established libraries or frameworks.
Due to cookie storage limitations, this implementation is not suitable for large-scale or mission-critical data storage requirements.
Further Resources
For in-depth information on JavaScript cookies, refer to the official Mozilla Developer Network (MDN) documentation.

### Further Resources
For in-depth information on JavaScript cookies, refer to the official Mozilla Developer Network (MDN) documentation.

### Contributing
- Reporting Issues:
If you find a bug or have a suggestion, open an issue with clear details.

- Suggesting Improvements:
Share your ideas by opening an issue with a clear description.

- Submitting Pull Requests:
Contribute code by forking the repository, making changes, and submitting a pull request. Make sure to provide a clear description of your changes.

We appreciate your help in making this project better! 🚀

### License
This project is licensed under the Apache 2.0. License

