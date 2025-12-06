# UltiSnips Snippets 

Writing LaTeX mathematics can be tedious and time-consuming; but it need
not be so. 
Thanks to [Gilles Castel](https://castel.dev/post/lecture-notes-1/), it is
possible to quickly and effortlessly run through dense mathematics by using
snippets. For example, rather than writing
```latex
\[
\rho\left( \frac{\partial \mathbf{v}}{\partial t}
+\mathbf{v}\cdot \nabla \mathbf{v} \right)=-\nabla p+\nabla \cdot
\mathbf{T}+\mathbf{f}
.\]
```
one can write
```latex
dm
rho () part bfv <TAB> <TAB> t <TAB> + bfv <TAB> ** nabla bfv <TAB> <TAB> =
-nabla p + nabla ** bfT <TAB> + bff 
```
which saves time and saves trying to remember in which bracket nest one is
currently in (especially helpful for nested fractions
subscripts/superscripts).

I have modified the snippets file to my liking; but one can always modify
it to their preferences. The UltiSnips documentation is long and
unnecessary to read for the purposes of LaTeX snippets; simply look at the
way the snippets are defined in the file and it is clear how they work and
one can easily adapt or add their own from there. 

### How to use ###

*This assumes one writes LaTeX documents inside vim, for example using
VimTeX. In the same linked blog one can find out how to set it up.*

1. Install [UltiSnips](https://github.com/SirVer/ultisnips)
2. Create a directory `~/.vim/UltiSnips/`
3. Place `tex.snippets` in this folder and reload vim. 

Whenever you create a `.tex` file, it will know to use the snippets as
defined in the file; these snippets will not be called under a different
file extension. Examples of the cool things one can do can be found on the
blog that I linked at the top of this README. I have defined several other
snippets in addition. Some of the most useful are:

- `dm` to enter display math mode.
- `beg`: Use at the beginning of a line to create a `begin/end` environment
  of your choice. Press tab to cycle through. 
- `mk`: enter inline math mode.
- `frac` or `//` to create a fraction. Again press tab to cycle through
  numerator/denominator and to exit the brackets.
- `dint` for definite integrals.
- `sum` for summation
- `bf` for boldface math
- `EE` for expectation
- `tt` for math-mode text
- `part` for partial derivative
- `sr` and `cb` for squaring and cubing a term
- `td` expands to `^{}` for superscripts with more than one character
- `__` expands to `_{}` for subscripts with more than one character
- Every common variable name automatically adds a backslash. 
    - `vps` for `\varepsilon` and `eps` for `\epsilon`
- `**` for `\cdot` and `xx` for `\times`. 
- `sq` for square root
- `mcal` for `mathcal{}`
- Probably more, these are off the top of my head!

Thank you to Gilles Castel for having the creativity to think of this. He
was an incredibly gifted person and so kind to share his findings with the
broader community for free.

May he rest in peace. 
