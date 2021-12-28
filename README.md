## ethull's resume

Is a fork of [Awesome CV](https://github.com/posquit0/Awesome-CV) by posquit0.

Includes compatiblity changes so that a html resume can be generated with tex4ht, mainly:
- removes otf fonts as they are not supported
    - converts otf fonts to ttf with otf2ttf from [afdko](https://github.com/adobe-type-tools/afdko)
    - uses a fontawesome5 from ctan
    - applies tex4ht patch to fontawesome5 via .4ht config files (in future tex4ht src releases this wont be needed)

## setup tools
install texlive-full
- linux (ubuntu): follow this [guide](https://fahim-sikder.github.io/post/installing-texlive-latest-ubuntu) to install latest version
- for mac: brew install mactex

if fontawesome5 is not installed by default
- tlmgr install fontawesome5

## generate html or pdf output
    scripts/gen_html.sh
    scripts/gen_pdf.sh
