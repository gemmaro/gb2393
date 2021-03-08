File structure:

```
$ exa -Ta -I .git
.
├── .gitattributes
├── aaa
│  └── xxx.lll  # <- Git LFS target
├── bbb
│  └── yyy.txt  # <- NOT Git LFS target
└── README.md
```

The directories `aaa` and `bbb` (and the files they contain) should be included in the zip file,
but in fact only `README.md` and `.gitattributes` are included.

If you rename this file to `readme`, this file will not be included in the zip file either.
