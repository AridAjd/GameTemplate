# <div align="center">Introduction</div>
Hey there folks! Today's tutorial is a tidy bit more complex than how normal devforum tutorials are. We are going to look into external tooling, some in-depth explanation and tools that'll help you get the best of your skills!

# <div align="center">Why use external tooling?</div>
At first sight, external tooling seems very useless and some of you might even ask, "why do stuff outside roblox studio? It's just a hassle!!"

True enough, but if you think about it, Roblox Studio does not provide proper tools for development cases although it's somewhat manageable.

List of things Roblox Studio does not provide (at the time of writing this post):
- Version control
- Advanced code features
- Continuous Integration/Continuous Deployment (CI/CD) Support
- Cloud Collaboration (does not natively support more advanced cloud collaboration tools like real-time co-editing with conflict resolution besides team-create)

But, code-editing softwares like [VSCode](https://code.visualstudio.com/), [Sublime Text](https://www.sublimetext.com/), [Zed](https://zed.dev/) etc. can help you A LOT when you code because it provides you multiple extensions that helps to improve your code and your workflow. Adding on to that, you can even use CLI like windows terminal to run commands like `rojo` or `wally`. This reason right here, is why **I** personally recommend to code externally instead of in Roblox Studio.

Managing things at first may seem very hard, but when you get used to it, you can see it being much more helpful than Roblox Studio.

<div align="center">

# Required Tools

| Tool name | Comments |
| :-: | :-: |
| [Rokit](https://github.com/rojo-rbx/rokit) | To manage your tools like rojo or wally, you can use rokit. It's similar to [aftman](https://github.com/LPGhatguy/aftman) and [foreman](https://github.com/Roblox/foreman). |
| [Rojo](https://github.com/rojo-rbx/rojo) or [Argon](https://github.com/argon-rbx/argon) | Rojo or Argon can be used to sync your code from your code-editing software to Roblox Studio. |
| [Wally](https://github.com/UpliftGames/wally) | A well-known package manager in the Roblox community. |
| [Selene](https://github.com/kampfkarren/selene) | Used to lint your lua(u) code. |
| [StyLua](https://github.com/JohnnyMorganz/StyLua) | Used to style your lua(u) code. |
| [Rbxcloud](https://github.com/Sleitnick/rbxcloud) | Used to access the Roblox Open Cloud APIs. |
</div>

And obviously, we are going to be using [GitHub](https://github.com/) to host our game.

---

[details="What is GitHub?"]
GitHub is a web-based platform that hosts and manages code repositories using Git, a version control system. It allows developers to collaborate on projects, track changes, review code, and deploy software. With features like pull requests, issues, and continuous integration, GitHub is a central hub for software development and open-source projects.
[/details]

We can use GitHub to track the changes of our game including switching between releases and reverting back to a specific version if something goes wrong.

# <div align="center">Installing Rokit</div>
First of all, create a directory that you will use for your game.

Secondly, install [Rokit](https://github.com/rojo-rbx/rokit?tab=readme-ov-file#installation). This is as easy as it gets.

Next, to verify if rokit has installed, open your CLI (mine is Windows Terminal - Powershell) and open your that directory in your terminal. To open that directory, you can use the `cd` command (Change Directory) and enter the path. `cd [path]`

Then, type `rokit --version` or `rokit -V`

![image|233x124](upload://godKsgjVI7JMwuzkxNudAHxkqTW.png)

Next, initialize the rokit file using `rokit init` and it should create a `rokit.init` file in your game's directory.

[details="Install the required tools with the following commands"]
```
rokit add rojo-rbx/rojo
rokit add argon-rbx/argon # Install either rojo or argon.
rokit add UpliftGames/wally
rokit add Kampfkarren/selene
rokit add JohnnyMorganz/StyLua
rokit add Sleitnick/rbxcloud
```
[/details]