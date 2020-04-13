# Simple Javascript ES6 - Starter


Simple Javascript ES6 template compressing JS code into a single bundle file.

## Installation

Required tools
```bash
NODEJS and NPM or YARN (JS package manager)
```

Using NPM, execute the below code on your project folder.
It will create a package.json file on your directory. (package.json file will have all your project's dependencies in one file.

```bash
npm init
```

After that, we will need BABEL, run the following commands on your project folder.

```bash
npm add @babel/cli
```
```bash
npm add @babel/preset-env
```
```bash
npm add @babel/core
```

Create the file '.babelrc' on your project's root.

```bash
touch .babelrc
```

Save the file with the following code. (Preset-env defines our env, so it rends our code in a way browsers can understand).

```bash
{
    "presets": ["@babel/preset-env"]
}
```

Open package.json and add a new script value. It executes babel using our main.js file and creating our bundle.js. The -w flag is used to track the changes on our main.js  and generate a new bundle.js everytime we change something.

```bash
"scripts": {
    "dev": "babel ./main.js -o ./bundle.js -w"
},
```

## Usage

You can use the following code to start your development, our babel will watch our project for changes and generate the bundle file, enjoy!!!

```bash
npm run dev
```

You can now start your project the way you want, bundle will generate all your javascript code in a way browsers can understand. It's a simple JS starter project, for study purposes.


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)