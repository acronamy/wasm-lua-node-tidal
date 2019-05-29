# wasm-lua-node-tidal

Welcome to my experiment, you will find most of the emscripten compiler commands in npm package.json "config". There is also a installer task for lua built in.

## Requirements
#### compiler:
emscripten 1.38.30^
#### runtime:
node 10.0.0^
#### build tools:
- make
- curl

### Building
1. `npm run install-lua`
The task install-lua will go ahead and download a copy of lua 5.3.5 which is the latest stable.
Compile with emscripten.
Rewire the emscripten js gluecode.
Run `index.js`

#### Compile only
To just compile use `npm run compile`.
#### run only
To just run use `npm start`

---

## What is working
- Return flat lua tables to node!

### What isnt working.
- returning strings and numbers (simple TODO)

### Todo
- Unit testing with Jest
- Return strings
- Return nil as null
- Return dobules as number
- Return nested tables
- Returning functions ?!
- Improve nodelike Lua require to search paths lua_modules
- Integrate lua-rocks and wrap so that installs are more node like
- Test and validate fresh installs and install scripts
- Reduce and remove c++ dependencies where posible
- General repo management
- Create branding, website docs and RC.alpha-1

[Inspiration | https://github.com/vvanders/wasm_lua] by the fantastic @vvanders