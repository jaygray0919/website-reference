# Installation Notes

## Install gulp

## Install other dependencies

  1. Install the LTS version of Node.js.

    `nvm install --lts`

  2. Install Python 2.7

    *Currently running:* `Python 2.7.6`

```
echo "export PATH=\"$(python -m site --user-base)/bin\":\$PATH" >> ~/.bashrc
source ~/.bashrc
sudo apt install -y python-yaml
```

  3. Install Grow

    `pip install --user grow`

    *successful*

## Fork & clone the repository

`git clone https://github.com/jaygray0919/amp.dev`

... and then install the dependencies via NPM:

`cd amp.dev`

`npm install`

## Notes

`npx gulp buildComponentVersions`

`npx gulp buildBoilerplate`

    `failed`
  
`npx gulp buildPlayground`

    `failed`

`npx gulp importAll --queue-imports`

    `failed`

`npx gulp buildSamples`

`command failed: git config user.name`

`at /amp.dev/gulpfile.js/build.js:33:13`


## EXPLANATION about user.name
- [link: Stackoverflow; Git configuration user.name doesn't work](https://stackoverflow.com/questions/25593043/git-configuration-user-name-doesnt-work)
- [link: problem with installing amp.dev](https://github.com/ampproject/amp.dev/issues/4163)
