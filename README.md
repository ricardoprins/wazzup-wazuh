# Wazzup Wazuh! :detective:

> **_“Just because we’re monitoring, doesn’t mean we’re not having fun."_** _– Michael Scott if he worked in cybersecurity_

![The Office quote](7rl4ga.jpg)

Welcome to Wazzup Wazuh, a delightfully simple setup for the Wazuh security platform using Docker. This repository was forged in the fires of Mount Doom, navigated the Death Star exhaust port, and once beat Dwight Schrute at a beet-growing contest. Brought to you by Ricardo Prins, it's licensed under the MIT License and open for contributions.

> "You have my sword. And my bow. And my Wazuh." :crossed_swords:

Wazuh is an open-source security platform that brings together host-based security monitoring and threat detection. It’s like the Fellowship of the Ring, but for cybersecurity. Whether you’re battling Balrogs or Sith Lords, Wazuh has your back.

For more about Wazuh, visit the [Wazuh website](https://wazuh.com/).

> "Help me, Obi-Wan Kenobi. You're my only hope." :space_invader:

This setup is designed to run on a Docker environment. Docker is like the Millennium Falcon of software: It may not look like much, but she’s got it where it counts.

Here's how you can get your Docker environment up and running faster than Han Solo's Kessel Run:

### Windows

> _"I'm not superstitious, but I am a little stitious."_

1. Visit the [Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/) download page.
2. Click "Get Docker".
3. Run the installer.
4. Enjoy your newfound power.

### MacOS

> _"May the Docker be with you."_

1. Head to the [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/install/) download page.
2. Click "Download Docker Desktop for Mac".
3. Run the installer.
4. Show the world that Macs aren’t just for graphic design.

### Linux

> _"One Docker to rule them all."_

1. Check the [Docker Engine overview](https://docs.docker.com/engine/install/) for your specific Linux distribution instructions.
2. Install Docker Engine using the appropriate commands.
3. Bask in the glory of your Linux prowess.

> "I'm ready to face any challenge that might be foolish enough to face me." :muscle:

Now that you're equipped with Docker, it's time to deploy the Wazuh platform. You can do this by cloning this repository and using Docker Compose. Here's a guide that even Kevin Malone could follow:

```bash
# Clone the repository
git clone https://github.com/ricardoprins/wazzup-wazuh.git

# Go to the directory
cd wazzup-wazuh

# Run Docker Compose
docker-compose up -d
```

## Running the Show (Configuration)

> "You miss 100% of the shots you don't take." - Wayne Gretzky - Michael Scott - Docker :basketball:

So you've cloned the repository and you're eager to start. Your next step is to enter the vast and exciting world of Docker Compose! But don't worry, it's easier than making a decent cup of coffee in the Dunder Mifflin break room.

First, you're going to need to create a `.env` file to store environment variables (I've added a .env.example file that you can just copy/paste/rename if you want). It's a bit like your own personal R2-D2, carrying your most vital data. In the main directory of your cloned repository (that would be `wazzup-wazuh`), create a file called `.env` and add the following lines:

```
PUID=1000
PGID=1000
NGINX_PORT=443
NGINX_PWD=<your-desired-password>
```

Replace `<your-desired-password>` with your chosen password for the Nginx server. And keep it secret. Keep it safe. Maybe don't go as far as tossing it into Mount Doom, but definitely don't write it on a Post-it note and stick it to your monitor. Unless, of course, you want an unexpected visit from the Dark Lord (or, worse, Toby from HR).

Once you've done that, simply navigate to the directory (as though you're journeying through Middle-earth, but without the orcs) in your terminal, and run the following command:

```
docker-compose up -d
```

And voilà! You've just instructed Docker to create your environment in detached mode, faster than the Millennium Falcon on a good day.

You might not be declaring a thumb war or leading an Ewok village, but in the world of cybersecurity, you're pretty much a hero now. Remember, “Do or do not. There is no try.” And you've definitely done it!

Take a moment to enjoy this accomplishment. Breathe. Maybe eat a beet. Or a donut. You've earned it.

And remember: "Your focus determines your reality" – Qui-Gon Jinn, and probably someone from IT, too.

---

I hope you find this helpful! Welcome to the magical world of Docker and Wazuh!

> "The Force will be with you. Always." :sparkles:

For any issues, feel free to raise an issue on GitHub, or send a raven, lightsaber, or paper airplane. I'm always open for collaboration and contributions. After all, "many hands make light work." That's Elvish, right?

For more of my work and thoughts, check out my blog at [ricardoprins.dev](https://ricardoprins.dev).

> _"If you don’t like it, Stanley, you can go to the back of the bus."_ Or just fork the repo. That works too.
