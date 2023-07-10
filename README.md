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

**NOTE: This doesn't work on Macs with ARM chips.**

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

# Generate SSL certs
docker-compose -f generate-indexer-certs.yml run --rm generator

# Evoke the final magic script
docker-compose up -d
```

## Running the Show (Configuration)

> "You miss 100% of the shots you don't take." - Wayne Gretzky - Michael Scott - Docker :basketball:

Now, there's only one thing separating you from your Wazuh dashboard.

Open your browser, navigate to https://localhost, and input the user/password combination

(the default values are admin:SecretPassword - these can be changed in the wazuh_indexer\internal_users.yml file)

---

I hope you find this helpful! Welcome to the magical world of Docker and Wazuh!

> "The Force will be with you. Always." :sparkles:

For any issues, feel free to raise an issue on GitHub, or send a raven, lightsaber, or paper airplane. I'm always open for collaboration and contributions. After all, "many hands make light work." That's Elvish, right?

For more of my work and thoughts, check out my blog at [ricardoprins.dev](https://ricardoprins.dev).

> _"If you don’t like it, Stanley, you can go to the back of the bus."_ Or just fork the repo. That works too.
