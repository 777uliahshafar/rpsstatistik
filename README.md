# SIMART TEMPLATE
This template was created using article class in 10/11/2020. The purpose of this template is to create fabolous article. With the help of helpers4ht, the configuration of this template can turn the compilation to HTML. In case we need to create word file, we can easly copy text from html file.

## Change compiler engine
% Add this line below to the first fifth line in begginning main file. Specify the compiler engine.


`%! TeX program = pdflatex ` for pdflatex
or
`%! TeX program = lualatex` for LuaLatex(reccomend)



#Convert Lualatex to HTML
This template has already been configured with helpers4ht in mycfg file. Some style of text required package which can be activated in preamble main.tex.

## Install
Install Helpers4ht

`mkdir -p $(kpsewhich -var-value TEXMFHOME)/tex/latex`

This will create directory ~/Library/texmf/tex/latex.

`git clone https://github.com/777uliahshafar/helpers4ht.git`


## Compile HTML

`make4ht -ul filename "configfilename"`

-u = compile with encoing utf-8
-l = cimpile with lualatex engine
