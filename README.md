# MLAdy Documentation

📄 [**TIN301** - Design Report and Basis for Funding](TIN301.md)

## 🚀 QUICK START:

_Note: Only tested on Windows 10_

[Install VSCode](https://code.visualstudio.com/)

[Install Pandoc](https://pandoc.org/installing.html)

[Install Markdown Preview Enhanced (VSCode extension)](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

[Install Pandoc Citer (VSCode extension)](https://marketplace.visualstudio.com/items?itemName=notZaki.pandocciter)

[Install MiKTeX](https://miktex.org/download)

Preprocess document:  
_[Tip: Pandoc command-line options](https://pandoc.org/MANUAL.html#default-files)_

```sh
pandoc TIN301.md -o "temp.md" -A bottom.md
```

Export to `.docx`-format (Word) in terminal:

```sh
pandoc temp.md -o "TIN301.docx" --citeproc --metadata-file TIN301.yaml --reference-doc design.docx
```

## 📖 USEFUL GUIDES AND RESOURCES:

- [Chrome extension to quickly get BibTex-reference from websites](https://chrome.google.com/webstore/detail/bibtex-entry-from-url/mgpmgkhhbjgkpnanlmlhibjfgpdpgjec?hl=en)
- [Pandoc manual](https://pandoc.org/MANUAL.html)
- [Pandoc examples](https://pandoc.org/demos.html)
- [Pandoc and citations](https://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
- [Automatic URL citation](https://phiresky.github.io/blog/2019/pandoc-url2cite/)
- [Writing GitHub-markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Guide on GitHub markdown to scientific-paper](https://gist.github.com/maxogden/97190db73ac19fc6c1d9beee1a6e4fc8)
