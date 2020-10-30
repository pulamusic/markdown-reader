> Jim Carroll |
> 10/30/2020 |
> [GitHub Profile](https://github.com/pulamusic)

---

# tree outputs



---

#### a tree map of the project directories after installing `marked` with `npm`

```zsh
% tree -d

.
├── assets
│   └── img
├── node_modules
│   └── marked
│       ├── bin
│       ├── lib
│       ├── man
│       └── src
├── scripts
└── styles
    ├── css
    └── scss

12 directories
```

all right, I'll try the -a flag instead, but I'll output it to a .txt file.

`tree -a >> tree-1.txt`

It worked great. ~~It's a bit longish for a `README.md` file.~~ See `./tree-1.txt`. 13 directories, 31 files.

---

#### all files and folders after `npm install marked --save`

```zsh
$ tree -a >> tree-1.txt

.
├── .gitignore
├── LICENSE.md
├── README.md
├── assets
│   └── img
├── index.html
├── index.js
├── node_modules
│   ├── .bin
│   │   └── marked -> ../marked/bin/marked
│   └── marked
│       ├── LICENSE.md
│       ├── README.md
│       ├── bin
│       │   └── marked
│       ├── lib
│       │   ├── marked.esm.js
│       │   └── marked.js
│       ├── man
│       │   ├── marked.1
│       │   └── marked.1.txt
│       ├── marked.min.js
│       ├── package.json
│       └── src
│           ├── Lexer.js
│           ├── Parser.js
│           ├── Renderer.js
│           ├── Slugger.js
│           ├── TextRenderer.js
│           ├── Tokenizer.js
│           ├── defaults.js
│           ├── helpers.js
│           ├── marked.js
│           └── rules.js
├── package-lock.json
├── package.json
├── scripts
│   └── main.js
├── styles
│   ├── css
│   │   └── main.css
│   └── scss
│       └── main.scss
└── tree-1.txt

13 directories, 31 files
```

---
