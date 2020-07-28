# Markdown sample
|100-200-300|400-500-600|700-800-900|
|------------- |---------------| -------------|
|<span class="w100">markdown 100 字重</span>|<span class="w400">markdown 400 字重</span>|<span class="w700">markdown 700 字重</span>|
|<span class="w200">markdown 200 字重</span>|<span class="w500">markdown 500 字重</span>|<span class="w800">markdown 800 字重</span>|
|<span class="w300">markdown 300 字重</span>|<span class="w600">markdown 600 字重</span>|<span class="w900">markdown 900 字重</span>|

- list a
- list b

---

<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
[連結](https://www.apple.com)

| Left Aligned  | Center Aligned  | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is      | some wordy text |         $1600 |
| col 2 is      | centered        |           $12 |
| zebra stripes | are neat        |            $1 |


## Markdown and I
**Markdown 馬克檔** is a plain text formatting syntax created by John Gruber, aiming to provide a easy-to-read and feasible markup. The original Markdown syntax specification can be found [here](http://daringfireball.net/projects/markdown/syntax). 連結顏色不一樣？
## Markdown and I
Codepen editor.

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

### Links and Email
#### Inline
Just put angle brackets around an email and it becomes clickable: <uranusjr@gmail.com>  
`<uranusjr@gmail.com>`  

Same thing with urls: <http://macdown.uranusjr.com>  
` <http://macdown.uranusjr.com>`

### Lists

* Lists must be preceded by a blank line (or block element)
* Unordered lists start each item with a `*`
- `-` works too
	* Indent a level to make a nested list
		1. Ordered lists are supported.
		2. Start each item (number-period-space) like `1. `
		42. It doesn't matter what number you use, I will render them sequentially
		1. So you might want to start each line with `1.` and let me sort it out

### Block Quote

> Angle brackets `>` are used for block quotes.  
Technically not every line needs to start with a `>` as long as
there are no empty lines between paragraphs.  
> Looks kinda ugly though.
> > Block quotes can be nested.  
> > > Multiple Levels
>
> Most markdown syntaxes work inside block quotes.
>
> * Lists
> * [Links][arbitrary_id]
> * Etc.

### <a name="fenced-code-block">Fenced Code Block</a>

This is a fenced code block:

```
print ('Hello world!)'
```

```C++
printf ("hellow world!!!")
```

You can also use waves (`~`) instead of back ticks (`` ` ``):

~~~
print('Hello world!')
~~~

### Inline Formatting

The following is a list of optional inline markups supported:

Option name         | Markup           | Result if enabled     |
--------------------|------------------|-----------------------|
Intra-word emphasis | So A\*maz\*ing   | So A<em>maz</em>ing   |
Strikethrough       | \~~Much wow\~~   | <del>Much wow</del>   |
Underline [^under]  | \_So doge\_      | <u>So doge</u>        |
Quote [^quote]      | \"Such editor\"  | <q>Such editor</q>    |
Highlight           | \==So good\==    | <mark>So good</mark>  |
Superscript         | hoge\^(fuga)     | hoge<sup>fuga</sup>   |
Autolink            | http://t.co      | <http://t.co>         |
Footnotes           | [\^4] and [\^4]: | [^4] and footnote 4   |

[^4]: You don't have to use a number. Arbitrary things like `[^footy note4]` and `[^footy note4]:` will also work. But they will *render* as numbered footnotes. Also, no need to keep your footnotes in order, I will sort out the order for you so they appear in the same order they were referenced in the text body. You can even keep some footnotes near where you referenced them, and collect others at the bottom of the file in the traditional place for footnotes. 

### TeX-like Math Syntax
I can also render TeX-like math syntaxes, if you allow me to.[^math] I can do inline math like this: \\( 1 + 1 \\) or this (in MathML): <math><mn>1</mn><mo>+</mo><mn>1</mn></math>, and block math:

\\[
    A^T_S = B
\\]

or (in MathML)

<math display="block">
    <msubsup><mi>A</mi> <mi>S</mi> <mi>T</mi></msubsup>
    <mo>=</mo>
    <mi>B</mi>
</math>

##### Task List Syntax
1. [x] I can render checkbox list syntax
	* [x] I support nesting
	* [x] I support ordered *and* unordered lists
2. [ ] I don't support clicking checkboxes directly in the html window

![MacDown Screenshot](https://d.pr/i/10UGP+)
---
*Emphasize*: `*Emphasize*` or `_Emphasize_`[^emphasize] (Command-I)

[^emphasize]: If **Underlines** is turned on, `_this notation_` will render as underlined instead of emphasized 

---

x~z,y~

![This is the figure caption][fig_id]

[fig_id]: mmd.png "This is where the title goes" height=45px width=120px

---
