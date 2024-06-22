# FiveM Loading Screen Standalone

Welcome to the FiveM Loading Screen Standalone repository! This project is designed to enhance the loading experience for your FiveM server, supporting both ESX and QBcore frameworks. With the ability to add custom functions, you can play multiple background videos and display interactive buttons for a dynamic and engaging loading screen.

## Author
Created By [@ZAID](https://fiverr.com/users/zaidqaiser3)


## Preview
![1](https://github.com/zaidqaiser/FiveM-LoadingScreen--Latest/assets/114343092/bcf137ee-d5d0-4356-b57d-842e42c4876b)

## Features

- **Multi-Video Background**: Play more than one video in the background to keep your players entertained while they wait.
- **Framework Compatibility**: Fully compatible with both ESX and QBcore frameworks.
- **Custom Functions**: Easily add custom functions to enhance the loading screen's interactivity and functionality.
- **Interactive Buttons**: Display buttons on the screen to provide useful information or actions for the players.
- **User-Friendly Configuration**: Simple and easy-to-understand configuration files to get you up and running quickly.

## Installation

1. Clone the repository to your FiveM server's resources directory.
    ```bash
    git clone https://github.com/yourusername/fivem-loading-screen-standalone.git
    ```

2. Add the resource to your server configuration file (`server.cfg`).
    ```plaintext
    start fivem-loading-screen-standalone
    ```

3. Configure the loading screen by editing the `config.js` file to suit your server's needs.

## Configuration

The `config.js` file allows you to customize various aspects of the loading screen. You can add multiple video URLs, configure button texts and actions, and tailor the screen's appearance to match your server's theme.

### Sample Configuration

Below is a sample configuration file (`config.js`) to get you started:

```javascript
Config = {}; // Don't touch

Config.ServerIP = "localhost:30120";

// Social media buttons on the left side
Config.Socials = [
    {name: "discord", label: "Discord", description: "Join our community, have fun!", icon: "assets/media/icons/discord.png", link: "https://discord.gg/#"},
    {name: "tiktok", label: "Tiktok", description: "Watch our video here!", icon: "assets/media/icons/tiktok.png", link: "https://www.instagram.com/#"},
    {name: "Paypal", label: "Instagram", description: "Checkout latest Update or Events!", icon: "assets/media/icons/tebex.png", link: "https://www.instagram.com/#"},
];

Config.HideoverlayKeybind = 112 // JS key code https://keycode.info
Config.CustomBindText = "F1"; // leave as "" if you don't want the bind text in html to be statically set

// Staff list
Config.Staff = [
    {name: "Staff#1", description: "Name", color: "#fff", image: "https://cdn.discordapp.com/attachments/1127485698354716723/1253979300420649011/logo.png?ex=6677d2bb&is=6676813b&hm=972cc87d3da1db0c7b727f3cc51c0a0e4c21bd394edf1cc1433399f3abd2f0c7&"},
    {name: "Staff#2", description: "Name", color: "#fff", image: "https://cdn.discordapp.com/attachments/1127485698354716723/1253979300420649011/logo.png?ex=6677d2bb&is=6676813b&hm=972cc87d3da1db0c7b727f3cc51c0a0e4c21bd394edf1cc1433399f3abd2f0c7&"},
    {name: "Staff#3", description: "Name", color: "#fff", image: "https://cdn.discordapp.com/attachments/1127485698354716723/1253979300420649011/logo.png?ex=6677d2bb&is=6676813b&hm=972cc87d3da1db0c7b727f3cc51c0a0e4c21bd394edf1cc1433399f3abd2f0c7&"},
    {name: "Staff#4", description: "Name", color: "#fff", image: "https://cdn.discordapp.com/attachments/1127485698354716723/1253979300420649011/logo.png?ex=6677d2bb&is=6676813b&hm=972cc87d3da1db0c7b727f3cc51c0a0e4c21bd394edf1cc1433399f3abd2f0c7&"},
];

// Categories
Config.Categories = [
    {label: "Social Networks", default: false},
    {label: "Staff team", default: true}
];
```

## Contributing
We welcome contributions from the community! Feel free to fork the repository, make improvements, and submit pull requests. Please ensure your code follows the project's coding standards and includes relevant documentation.

## Support
If you encounter any issues or have questions, please open an issue on the GitHub repository, and we'll be happy to assist you.
