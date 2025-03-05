# UltiSnips Snippets 

For `.tex` and `.md` files, I use the following snippets 
(`markdown.snippets`) is still young. 
I have taken the majority of my snippets from Gilles Castel
and [here](https://github.com/honza/vim-snippets/blob/master/UltiSnips/markdown.snippets). 

# How to use #

1. Install [UltiSnips](https://github.com/SirVer/ultisnips). 
2. Create a directory `~/.vim/UltiSnips/`        
3. Place `markdown.snippets` and `tex.snippets` in this folder
and reload Vim (just close your terminal and open it again).

Now whenever you run 
```bash
vim file.md
```
or
```bash
vim file.tex
```
you can use UltiSnips snippets that are defined in the files.

# Examples #

- In a `.tex` file, you can type `f` followed by `<TAB>` and it will
expand to create a basic document.
    - You can write `beg` and it will create
    ```LaTeX
    \begin{|}

    \end{|}
    ```
    with your cursor placed in the brackets; it will mirror what you write
    in the top on the bottom. After pressing `<TAB>` it will place
    your cursor in between the delimiters. 
    - In math mode (e.g., `dm` for display math; `mk` for inline math),
    you can write `//` to create `\frac{}{}` and it will place your
    cursor in the first brackets; after pressing `<TAB>` it will move
    your cursor to the next brackets.
    - `ali` for an aligned environment
    - Many, many more. See Gilles Castel's blog for more examples. 
- I recommend reading the files to determine how they are used. 
UltiSnips has extensive documentation, but it's not necessary to read
it for most purposes; just look at the files themselves and learn
the syntax by trial and error. It's very easy and soon you will be able to create your 
own snippets according to your needs. 

