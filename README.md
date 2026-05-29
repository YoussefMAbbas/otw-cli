<p align="center">
  <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fthanoskoutr.com%2Fcovers%2Foverthewire.jpg&f=1&nofb=1&ipt=910f2eeba2af2cd177288c1db80b2209ec69701f9a2880e9899c15884b9167c2"
       alt="OverTheWire Banner"
       width="250">
</p>

<h1 align="center">OverTheWire CLI a cooler way to connect to wargames</h1>

<p align="center">
A Bash script that connects users to OverTheWire CTF games directly from the terminal. Fetches and parses game data from JSON to list available wargames, levels, and updates in a fast, terminal-friendly interface.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OverTheWire-CLI-orange">
  <img src="https://img.shields.io/badge/Focus-OTW%20CTF-red">
  <img src="https://img.shields.io/badge/Type-CLI%20Script-success">
</p>

<table>
<tr>
<th>
SSH Based Games
</th>
<td>
  <img src="./assets/ssh_games_preview.gif" alt="ssh_preview gif">
</td>
<th>
WEB Based Games
</th>
<td>
  <img src="./assets/web_games_preview.gif" alt="web_preview gif">
</td>
</tr>
</table>

---

## 📑 Table of Contents

- [About OTW-CLI](#-about-otw-cli)
- [Prerequisites](#-prerequisites)
- [Usage Example](#usage-example)
- [Contributing](#-contributing)
- [Connect With Me](#-connect-with-me)
- [Why This Repository Exists](#-why-this-repository-exists)

---

## 📌 About OTW-CLI

`otw` is a lightweight shell script that streamlines access to the [OverTheWire](https://overthewire.org) wargames platform.
It provides an interactive terminal interface for selecting games and levels, automatically handling SSH connections, browser launches, and game metadata retrieval.

Designed for convenience and speed, the script supports both terminal-based and web-based wargames such as `Bandit`, `Leviathan`, `Natas`, and more all from a single command.

### Features

- Interactive game and level selection
- Automatic SSH login using `sshpass`
- Browser integration for web wargames
- Dynamic game list fetched from OverTheWire
- Optional terminal image/banner rendering with `imgcat` or `jp2a`
- Minimal dependencies and portable POSIX-style shell workflow

---

## 📋 Prerequisites

You should have:

- `bash`
- `ssh`
- `sshpass` required for wargame password authentication
- `jq` used to fetch and parse game data from JSON
- `$BROWSER` environment variable pointing to your preferred browser (used by the `Natas` and `BlackSun` wargames)
- Optional: `imgcat` _(recommended)_ or `jp2a` for rendering a nicer banner in the terminal

---

## 🚀 Usage Example

Launch the OverTheWire helper script:

```bash
./otw
```

Example session:

```text
$ ./otw

============================
: Pick Your Poison :

00 - bandit
01 - krypton
02 - leviathan
03 - natas
04 - vortex
============================

* Enter game name: bandit

 : Getting game info :

* Enter level (0-34): 0
* Enter level password:

Connecting to the game...

bandit0@bandit.labs.overthewire.org's password:
```

### For a web-based games

```text
* Enter game name: natas
* Enter level (0-34): 5
```

This automatically opens:

```text
http://natas5.natas.labs.overthewire.org
```

---

## 🤝 Contributing

If you have:

- Optimization suggestions
- Additional features

Feel free to open an issue or submit a pull request.

---

## 💬 Connect With Me

If you're also working on scripts or interested in CTFs, feel free to connect.

<a href="https://youssefmabbas.medium.com/">![Medium](https://img.shields.io/badge/Medium-black?style=for-the-badge&logo=medium)</a>
<a href="https://www.linkedin.com/in/youssefmabbas/">![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)</a>
<a href="mailto:youssefmabbasofficial@proton.me">![Protonmail](https://img.shields.io/badge/ProtonMail-8B89CC?style=for-the-badge&logo=protonmail&logoColor=white)</a>

---

## ⭐ Why This Repository Exists

This project serves as:

- A fast and easy way to connect to games through the terminal
- Makes the CTFs more fun this way
