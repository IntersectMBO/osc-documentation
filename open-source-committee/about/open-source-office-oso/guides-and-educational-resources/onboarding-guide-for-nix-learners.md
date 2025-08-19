---
description: >-
  This page is in active construction and welcome to feedback for any
  inaccuracies.
---

# 😅 Onboarding Guide for Nix Learners

### Why Learn Nix?

Nix is a novel, _functional_ package manager and build tool focused on **reproducibility** and **isolation**. By design, Nix builds each package in a sandbox with explicit dependencies, so “if a package works on one machine, it will also work on another” [nixos.org](https://nixos.org). In practice this means you can define your entire development or deployment environment in plain-text Nix files and rebuild it exactly, byte-for-byte, on any Linux or macOS machine [nixos.org](https://nixos.org)[brodrigues.co](https://brodrigues.co/posts/2023-07-13-nix_for_r_part1.html). For example, one user notes that “Nix lets me have multiple projects on the same system that each have their own independent view of what dependencies are available” [mtlynch.io](https://mtlynch.io/notes/nix-dev-environment/) – you can run an old Python 2.7 project and a new Python 3 project side-by-side without conflict. Nix also ensures **atomic upgrades and rollbacks**: installing or updating a package never overwrites others, and you can instantly roll back if something breaks [nixos.org](https://nixos.org/guides/how-nix-works/). In short, Nix eliminates “it works on my machine” issues by making your environment _declarative_ (all tools and versions are described in code) and _reproducible_ [nixos.org](https://nixos.org)[brodrigues.co](https://brodrigues.co/posts/2023-07-13-nix_for_r_part1.html).

### Who This Guide Is For

This guide is for **developers and contributors** eager to use Nix for reproducible builds and environments. You might be a programmer learning Nix for the first time, a data scientist who needs consistent tool versions, or an open-source maintainer seeking declarative deployment. No prior Nix experience is assumed – if you know basic Unix command-line usage and care about reproducibility, you’re the right audience. (Nix works on Linux and macOS, and can even be used in Windows via WSL2.) Ultimately, **anyone** who wants reliable, shareable development environments – from students to DevOps engineers – will benefit from Nix.

### Getting Started

The easiest way to install Nix is via the official installer script. On **Linux** (with `systemd`), run the multi-user installer as root or with `sudo`:

```bash
bashCopyEdit$ sh <(curl --proto '=https' --tlsv1.2 -L https://nixos.org/nix/install) --daemon
```

This creates `/nix/store` and adds the `nix` command to your shell profile [nixos.org](https://nixos.org/download/). On **macOS**, the same script works (without `--daemon` by default); open Terminal and run:

```bash
bashCopyEdit$ sh <(curl --proto '=https' --tlsv1.2 -L https://nixos.org/nix/install)
```

Then restart your shell or source the profile to get `nix` in your PATH [nixos.org](https://nixos.org/download/). On **Windows**, install Nix inside WSL2 with systemd enabled: enable systemd (per Microsoft’s guide) and run the installer (with `--daemon` if desired) [nixos.org](https://nixos.org/download/). After installation, you can verify by running `nix --version` or `nix-env --version`.

_Optional configuration:_ To use Nix’s new “flakes” feature for reproducible projects, you’ll need to enable it in your Nix config. For example, add this line to `~/.config/nix/nix.conf`:

```
iniCopyEditexperimental-features = nix-command flakes
```

or always run Nix with `--experimental-features 'nix-command flakes'`[tweag.io](https://www.tweag.io/blog/2020-05-25-flakes/). This lets you use commands like `nix flake init` and `nix develop` (covered below).

> **Tip:** Read the Nix manual’s _Quick Start_ or the NixOS manual for more details. The Nix download page provides the same instructions and links to the official docs [nixos.org](https://nixos.org/download/) [nixos.org](https://nixos.org/download/).

### First Steps

Once Nix is installed, try out its core commands and features:

* **`nix-shell` (ad-hoc development shells):** Run `nix-shell -p pkg1 pkg2 …` to drop into a temporary shell where those packages are available. For example `nix-shell -p hello git` starts a shell with `hello` and `git` installed. This is great for trying tools without installing them system-wide. For more complex cases, you can write a _shell expression_ in a file (e.g. `shell.nix`) to declare your environment, and then just run `nix-shell`. See the Nix tutorials for how to write `shell.nix` (for example, using `mkShell` or `mkShellNoCC`) to set up projects with all needed tools[nix.dev](https://nix.dev/tutorials/first-steps/declarative-shell.html)[nix.dev](https://nix.dev/tutorials/first-steps/declarative-shell.html).
* **`nix-env` (per-user profiles):** You can install packages into your personal Nix profile. For instance, `nix-env -iA nixpkgs.hello` installs the `hello` package (via the Nixpkgs collection). Use `nix-env -qaP <pattern>` to search for packages. Newer Nix versions also have `nix profile install` (e.g. `nix profile install nixpkgs.hello`) which achieves the same in a more modern way. Your installed packages live in `~/.nix-profile`. To upgrade, run `nix-env --upgrade` (or `nix profile upgrade`). Since Nix keeps old versions, you can always roll back by `nix-env --rollback` if something goes wrong[nixos.org](https://nixos.org/guides/how-nix-works/).
* **Flakes (project pinning):** _Flakes_ are an optional Nix feature for reproducible projects. A _flake_ is a directory (often a Git repo) containing a `flake.nix` and `flake.lock`. You can create one with `nix flake init -t` or manually. A flake can define outputs like `devShells`, `packages`, or NixOS configurations. For example, a simple `flake.nix` might declare `devShells.default = mkShell { packages = [ pkgs.python39 pkgs.numpy ]; }`. Then running `nix develop` (or `nix shell .#default`) will load that environment. Because flakes use a lock file, all dependencies (even the Nixpkgs version) are pinned, ensuring reproducibility. Flakes are still marked experimental in some Nix releases, but they offer a clean way to share Nix setups with others [tweag.io](https://www.tweag.io/blog/2020-05-25-flakes/).
* **Home Manager (per-user config):** Home Manager is a Nix-based tool to manage your home directory (dotfiles, user services, personal packages) declaratively. After installing Nix, you can add the Home Manager channel and install it, then write a `home.nix` file describing your setup. For example, you might include `home.packages = [ pkgs.tmux pkgs.vim ];` and enable `programs.zsh.enable = true`. Running `home-manager switch` will apply your config. In fact, Home Manager “provides a radically better way to manage a user’s environment for both packages and dotfiles, effectively allowing you to take a configuration-as-code approach”ghedam.at. (It works on any Linux or macOS system with Nixghedam.at.) See the Home Manager manual or tutorials for step-by-step installation.

Each of these tools builds on the same core idea: write down _what_ you need in Nix language, and Nix takes care of fetching/building and isolating it. As one Nix user notes, even beginners can have fully Nix-managed dev environments in about 20 minutes [mtlynch.io](https://mtlynch.io/notes/nix-dev-environment/). In the next section we’ll list many learning resources to deepen your understanding.

### Learning Resources

There are many high-quality, beginner-friendly resources for Nix:

* **Official documentation and tutorials:** The NixOS website hosts guides and references. For example, _“How Nix Works”_ explains the core principles [nixos.org](https://nixos.org/guides/how-nix-works/) [nixos.org](https://nixos.org/guides/how-nix-works/). The _Nix Pills_ tutorial series is a classic introduction on nixos.org [nixos.org](https://nixos.org/guides/nix-pills/). The NixOS/Nix manual pages cover commands like `nix-shell` and Nix expressions. The nix.dev site (community-driven) has guided tutorials (e.g. setting up `shell.nix`) and a full reference.
* **Books and guides:** _NixOS & Flakes Book_ (free online) is an unofficial beginner book covering Nix and NixOS with examples [nixos-and-flakes.thiscute.world](https://nixos-and-flakes.thiscute.world). (Its preface even invites beginners: “Looking for a beginner-friendly tutorial? Then you've come to the right place!” [nixos-and-flakes.thiscute.world](https://nixos-and-flakes.thiscute.world).) Other recommended reads include _Nix Pills_ (as above) and _Nix Cookbook_ (paid). For advanced learning, _Learning Nix_ by Fumito Kowasaki (free) and various blog posts can help.
* **Tutorials and blogs:** Many community blogs and articles walk through Nix basics. For example, Michael Lynch’s blog shows how to set up per-project environments [mtlynch.io](https://mtlynch.io/notes/nix-dev-environment/). The blog _“Reproducible Data Science with Nix”_ by B. Rodrigues (July 2023) has a gentle intro to using Nix for R and data projects [brodrigues.co](https://brodrigues.co/posts/2023-07-13-nix_for_r_part1.html) [brodrigues.co](https://brodrigues.co/posts/2023-07-13-nix_for_r_part1.html). The official Tweag blog has a “Flakes” tutorial by Nix founder Eelco Dolstra [tweag.io](https://www.tweag.io/blog/2020-05-25-flakes/). Searching for “Nix tutorial” or “Nix pills” will turn up more guides.
* **Video and interactive:** YouTube has talks and tutorials from NixCon and community members (e.g. _“Nix for Beginners”_ playlists). The NixOS Wiki lists community-curated channels (see Nix Channels). For hands-on practice, sites like NixOS Playgrounds or Replit CoCalc let you run Nix examples in a browser.
* **Package search:** The Nixpkgs search or NixOS Packages Search is invaluable for finding Nix package names. The NixOS weekly newsletter summarizes latest news and blog posts.

Wherever possible, prefer official or well-maintained sources. The NixOS wiki and Discourse forums also maintain FAQs and tutorials. Try a few of these resources to find the explanations that suit you, and keep them handy as you learn.

### Tooling and Development Environment

Nix integrates with many developer tools and editors:

* **VS Code:** There’s a _Nix Environment Selector_ extension that can automatically switch your VSCode workspace to use a Nix shell [nixos.wiki](https://nixos.wiki/wiki/Visual_Studio_Code). You can also use the _direnv_ extension with nix-direnv to auto-load the shell for each project. The NixOS Wiki notes that you can use `nix-direnv` with the VSCode `direnv` extension, or the `nix-env-selector` extension for manual switching [nixos.wiki](https://nixos.wiki/wiki/Visual_Studio_Code). If you use VSCode on NixOS, you can install `vscode.fhs` or use the flatpak-based `/Applications` with a proper `NIXPATH`.
* **Direnv and Lorri:** For any shell or editor, the direnv tool works well with Nix. You can drop a `.envrc` in your project with `use nix` or `use flake`, and direnv will auto-load the environment. _Lorri_ is another tool that watches your `shell.nix` and rebuilds it when it changes, feeding updates to direnv in the background. As described on its homepage, “lorri is a `nix-shell` replacement for project development” with fast direnv integration [github.com](https://github.com/nix-community/lorri). After enabling `lorri` and `direnv` in your config, simply run `lorri init` in a project; from then on it will keep your dev environment in sync without blocking your terminal [github.com](https://github.com/nix-community/lorri).
* **Other editors:** Emacs users can use nix-emacs or `use-package` integrations to load environment automatically. Vim/Neovim users can rely on `vim-dispatch` with `nix-shell`. In general, any editor that launches a shell (e.g. for language servers) can benefit from a Nix shell environment. Many language LSP servers (Haskell, Rust, Python) work out-of-the-box once the tools are in the Nix shell.
* **Build tools:** You can use Nix with CI/CD as well. For example, GitHub Actions or NixOS GitLab CI templates show how to build Nix projects in pipelines. For containerized apps, Nix can produce Docker images deterministically.

Overall, the goal is to make Nix your _ambient environment_: code editors and terminals automatically use the Nix-defined versions of compilers, linters, etc., so you’re always running the right toolchain.

### Community and Support

Nix has an active, helpful community. Key places to get help:

* **Discourse (NixOS Forum):** The official NixOS Discourse forums (discourse.nixos.org) are the central Q\&A site. Ask questions, browse tutorials, or read the wiki. The NixOS website explicitly points new users to the forum for “Get in Touch” [nixos.org](https://nixos.org).
* **Matrix Chat:** The Nix community has Matrix (chat) rooms, e.g. `#nix` and `#nixos` on Matrix.org (accessible via matrix.to). You can ask questions in real time there. The NixOS site lists “Matrix Chat” as a primary contact option [nixos.org](https://nixos.org).
* **Reddit:** The subreddits /r/NixOS and /r/Nix have many users sharing tips and news. (Reddit is unofficial but often quick for beginner questions.)
* **GitHub:** Many Nix projects are on GitHub: in particular the Nixpkgs repo and the Nix repository itself. Browse their issue trackers or Discussions pages to see ongoing work and ask development-level questions. Reporting bugs or contributing fixes on GitHub is welcome once you’re more advanced.
* **StackOverflow:** The `nix` tag on StackOverflow has Q\&A for common problems, though coverage is spotty. For quick issues, Discourse or Matrix is usually faster.
* **Weekly newsletter and blog:** Keep an eye on the NixOS Weekly newsletter and the Nix blog for announcements, tutorials, and community news.

When asking questions, include relevant details (Nix version, system) and any Nix expressions you’re using. The community is generally very helpful to newcomers.

### Suggested First Projects

Hands-on practice will cement your Nix skills. Here are some ideas for starter projects:

1. **Reproduce a developer environment:** Pick a simple project in a language you know (e.g. a small Python or Node.js app). Write a `shell.nix` (or `flake.nix`) that provides the right compiler/interpreter and libraries. For example, make a Python `shell.nix` that loads Python 3 and `numpy`/`matplotlib`, then verify you can run your script. This shows off isolated, reproducible envs.
2. **Package a command-line tool:** Find a small open-source project (say, hello.c) and write a `default.nix` that builds it. You’ll learn how to use `stdenv.mkDerivation` or (easier) how to call `pkgs.makeShell`/`pkgs.runCommand` in a flake. Build it with `nix-build` and run the result in `./result/bin/hello`. Consider contributing it to Nixpkgs if it’s missing.
3. **Manage dotfiles with Home Manager:** Install Home Manager and move one of your config files (e.g. for `git` or your shell) under Nix management. Declare it in `home.nix` and run `home-manager switch`. This gets you familiar with Nix expressions for user config.
4. **Use Nix in a CI or Docker:** If you have a GitHub repo, try adding a GitHub Actions step that runs a Nix build. Or use Nix to create a Docker container: e.g. `nix-build '<nixpkgs/nixpkgs>' -A dockerTools.buildImage` with a simple NixOS config. This shows off Nix’s declarative deployment.
5. **Explore NixOS (optional):** If you’re adventurous, try the NixOS live ISO in a VM. It’s a full Linux distro entirely configured in Nix. Even if you stick to using Nix on another distro, seeing a system configured by Nix can deepen your understanding.

As you try these projects, consult the resources above when you get stuck. The key is to start small and expand: every time you tweak `shell.nix` or add a package to `nix-env` and see it build, you’ll learn something new. Welcome to the Nix ecosystem – enjoy the journey to reproducible, declarative environments!
