[![LinkedIn][linkedin-shield]][linkedin-url]
<!--
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


[![Github][github-shield]][github.com/zoumson?tab=repositories]
[![Stack Overflow][stackoverflow-shield]][stackoverflow.com/users/11175375/adam]
[![Leetcode][leetcode-shield]][eetcode.com/Hard_Code/]
-->
## CMakeLists Serie Number 4


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#file-structure">Files Structure</a>
      <ul>
        <li><a href="#folder">Folder</a></li>
        <li><a href="#entire-files-structure">Entire Files Structure</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->

Sample of CMakeLists with demos and libraries.

<!--Built with -->
### Built With

<br>

* [cmake](https://cmake.org/)
* [gnu](https://www.gnu.org/)

<br>

## File Structure

### Folder

* [include/](include/): c++ declarations.
* [src/](src/): c++ definitions.


### Entire Files Structure 

```
.
├── CMakeLists.txt
├── include
│   ├── lib1.h
│   └── lib2.h
├── README.md
└── src
    ├── demo
    │   ├── CMakeLists.txt
    │   ├── demo1
    │   │   └── demo1.cpp
    │   ├── demo2
    │   │   └── demo2.cpp
    │   └── demo3
    │       └── demo3.cpp
    └── lib
        ├── CMakeLists.txt
        ├── lib1
        │   └── lib1.cpp
        └── lib2
            └── lib2.cpp

9 directories, 11 files

```


<!-- GETTING STARTED -->
## Getting Started

This is a sample code of how you may configure CMakeLists with demos and libraries.
To get a local copy up and running follow these simple steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* cmake
  ```sh
  sudo apt-get install cmake
  ```
 

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/zoumson/CMakeLists.git
   ```
2. Go to the project directory source
   ```sh
   cd CMakeLists/_4_Multi-Demo_Multi-Lib 
   ```
3. Create empty directories `build`,  `lib`, and `bin`
   ```sh
   mkdir build  && mkdir bin && mkdir lib
   ```
4. Generate the libraries  and move them to `lib` and the exectutables then move them to `bin`
   ```sh
   cd build && cmake .. && make && cd ..
   ```  
<!-- USAGE EXAMPLES -->
### Usage

1. Run the executable `demo1`
```
./bin/demo1 
```
<br>

2. Expected output of `demo1`
```sh
CMakeLists serie number [4].
CMakeLists with multiple custom libraries and demos.
Calling from lib1.
```
3. Run the executable `demo2`
```
./bin/demo2
```
<br>

4. Expected output `demo2`
```sh
CMakeLists serie number [4].
CMakeLists with multiple custom libraries and demos.
Calling from lib2.
```   
5. Run the executable `demo3`
```
./bin/demo3
```
<br>

6. Expected output `demo3`
```sh
[ALL] libraries included.
CMakeLists serie number [4].
CMakeLists with multiple custom libraries and demos.
Calling from lib1.
CMakeLists serie number [4].
CMakeLists with multiple custom libraries and demos.
Calling from lib2.
```     
   
7. Back to the initial file structure configuration
   ```sh
   rm -r bin build lib
   ```
<!-- ROADMAP -->
## Roadmap

All the headers files are well docummented, read through the comments

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Adama Zouma - <!-- [@your_twitter](https://twitter.com/your_username) -->- stargue49@gmail.com

Project Link: [https://github.com/zoumson/CMakeLists](https://github.com/zoumson/CMakeLists.git)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Google](https://www.google.com/)
* [Stack Overflow](https://stackoverflow.com/)
* [Github](https://github.com/)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: linkedin.com/in/adama-zouma-553bba13a
[product-screenshot]: images/screenshot.png

