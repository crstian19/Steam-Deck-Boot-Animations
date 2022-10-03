# Steam-Deck-Boot-Animations

<a name="readme-top"></a>


[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/crstian19/Steam-Deck-Boot-Animations">
    <img src="https://seeklogo.com/images/S/steam-deck-logo-31A2A5AD56-seeklogo.com.png" alt="Logo">
  </a>

<h3 align="center">Steam Deck Boot Animations</h3>

  <p align="center">
    Compilation of boot animations created by the community.
    <br />
  </p>
</div>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Installation

1. You want to grab the video. make sure it's a webm file, 1280x800, 16:10 or it won't fit.
2. Get the video onto your deck, make a folder for it, if you want. keep it somewhere safe.
3. Navigate to **.local/share/Steam/steamui/movies** (this is where your video is going to end up.)
4. Open a terminal and exec 
   ```bash
   truncate -s 1840847 (filename.webm)
   ```
5.Rename your file to **deck_startup.webm** note: we want this to replace the original deck_startup.webm
6.Navigate to .local/share/Steam/steamui/css and open library.css, scroll to the bottom, find the line that contains “video{flex-grow:0....” and change it to
the following:
```css
video{flex-grow:1;width:100%;height:100%;z-index:10}
```
7.Save changes.

8.Open a terminal within /home/deck/.local/share/Steam/steamui/css and run the following
command:
```bash
truncate -s 38492 library.css
  ```




<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Thanks to the authors of the animations on reddit:

- [Zacketry](https://www.reddit.com/user/Zacketry)
- [BeefyDragon](https://www.reddit.com/user/BeefyDragon)
- [TareXmd](https://www.reddit.com/user/TareXmd)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/crstian19/Steam-Deck-Boot-Animations.svg?style=for-the-badge
[contributors-url]: https://github.com/crstian19/Steam-Deck-Boot-Animations/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/crstian19/Steam-Deck-Boot-Animations.svg?style=for-the-badge
[forks-url]: https://github.com/crstian19/Steam-Deck-Boot-Animations/network/members
[stars-shield]: https://img.shields.io/github/stars/crstian19/Steam-Deck-Boot-Animations.svg?style=for-the-badge
[stars-url]: https://github.com/crstian19/Steam-Deck-Boot-Animations/stargazers
