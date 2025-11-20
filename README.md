<div align="center">
  <a href="https://greasyfork.org/pt-BR/scripts/541297-instagram-follow-spy" title="Instagram Follow Spy" target="_blank">
    <img src="./assets/noun-spy-full_64.png" width="64" height="64" alt="Instagram Follow Spy" />
  </a>
</div>

<div align="center">

# Instagram Follow Spy

</div>

![repository-template-button](./assets/insta-spy-banner.png)

A [web scraper](https://en.wikipedia.org/wiki/Web_scraping) script for Instagram Web that allows you to find out who doesn't follow you and who you don't follow back, all through a pleasant and intuitive interface. You can also view the most recent analysis performed.

## Motivation

I took part as an instructor in a programming training program at a company where I worked. The focus of the challenge wasn’t on the functionality itself, but rather on showing beginners how to manipulate the DOM using *Vanilla JS*, through web scraping techniques.

## Usage

In your browser, install a script manager extension.

Suggestions:

- [Violentmonkey](https://violentmonkey.github.io) - *Recommended*
- [Tampermonkey](https://www.tampermonkey.net)
- [Greasemonkey](https://www.greasespot.net) - *Firefox only*


### Install from GreasyFork (*Recommended*)

Go to the [script page on GreasyFork](https://greasyfork.org/pt-BR/scripts/541297-instagram-follow-spy), then click the "Install this script" button and follow the installation process in your extension.

### Install from GitHub

Click on file `script.user.js`, then click `Raw` button to install it.

## Contributing

Contributors are welcome! :metal:

Please check out the [CONTRIBUTING](CONTRIBUTING.md).

You can also:

- :star2: give a star in this repository
- :heavy_heart_exclamation: share this project and recommending it to your friends

## Examples

Usage examples.

### Finding the Selector for the User List Container

Normalmente, os seletores sãos os mesmos tanto para o modal de Followers, quanto para o modal de Following.

1. Open the **Followers** or **Following** modal;
2. Inspect the element and find the main `div` of the modal;
3. Go down until you find the `div` responsible for the `scroll`;
4. Copy the style classes and replace them in the `FOLLOWERS_MODAL_LIST_CONTAINER_SELECTOR` and `FOLLOWING_MODAL_LIST_CONTAINER_SELECTOR` variables. Remember to keep the `div` selector together with the classes.

Step by step:
![modal-list-container-selector](./assets/find-modal-list-container-selector.gif)
