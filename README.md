# MLAdy Documentation

📄 [**TIN301** - Design Report and Basis for Funding]("TIN301 MLAdy.md")

## 🚀 QUICK START:

[Install VSCode](https://code.visualstudio.com/)

[Install Pandoc](https://pandoc.org/installing.html)

[Install Markdown Preview Enhanced (VSCode extension)](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

[Install Pandoc Citer (VSCode extension)](https://marketplace.visualstudio.com/items?itemName=notZaki.pandocciter)

Export to `.docx`-format (Word) in terminal:

```sh
pandoc "TIN301 MLAdy.md" -o "TIN301 MLAdy.docx" --reference-doc design.docx --citeproc --variable papersize=a4paper --extract-media cache
```

## 📖 USEFUL GUIDES AND RESOURCES:

- [Chrome extension to get BibTex-reference easily](https://chrome.google.com/webstore/detail/bibtex-entry-from-url/mgpmgkhhbjgkpnanlmlhibjfgpdpgjec?hl=en)
- [Pandoc Manual](https://pandoc.org/MANUAL.html)
- [Pandoc and citations](https://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
- [Automatic URL citation](https://phiresky.github.io/blog/2019/pandoc-url2cite/)
- [Writing GitHub-markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Guide on GitHub markdown to scientific-paper](https://gist.github.com/maxogden/97190db73ac19fc6c1d9beee1a6e4fc8)
