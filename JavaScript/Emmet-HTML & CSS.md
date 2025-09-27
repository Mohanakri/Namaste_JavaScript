# Emmet Cheat Sheet - HTML & CSS

## HTML Syntax

### Basic Elements
```
div → <div></div>
p → <p></p>
span → <span></span>
h1 → <h1></h1>
a → <a href=""></a>
img → <img src="" alt="">
ul → <ul></ul>
li → <li></li>
```

### Classes and IDs
```
div.container → <div class="container"></div>
p#intro → <p id="intro"></p>
div.header.main → <div class="header main"></div>
span.btn.btn-primary → <span class="btn btn-primary"></span>
```

### Attributes
```
a[href="#"] → <a href="#"></a>
img[src="image.jpg" alt="Image"] → <img src="image.jpg" alt="Image">
input[type="text" placeholder="Name"] → <input type="text" placeholder="Name">
div[data-id="123"] → <div data-id="123"></div>
```

### Nesting (Child: >)
```
nav>ul>li → <nav><ul><li></li></ul></nav>
div>p>span → <div><p><span></span></p></div>
header>nav>ul>li*3 → <header><nav><ul><li></li><li></li><li></li></ul></nav></header>
```

### Sibling (+)
```
div+p+span → <div></div><p></p><span></span>
h1+p → <h1></h1><p></p>
```

### Climb-up (^)
```
div>p>span^div → <div><p><span></span></p><div></div></div>
ul>li>a^^div → <ul><li><a href=""></a></li></ul><div></div>
```

### Multiplication (*)
```
li*3 → <li></li><li></li><li></li>
div.item*5 → <div class="item"></div>...(5 times)
ul>li*4 → <ul><li></li><li></li><li></li><li></li></ul>
```

### Grouping ()
```
(div>p)*3 → <div><p></p></div><div><p></p></div><div><p></p></div>
div>(header>h1)+(main>p)+(footer>span)
```

### Item numbering ($)
```
li.item$*3 → <li class="item1"></li><li class="item2"></li><li class="item3"></li>
div#item$*3 → <div id="item1"></div><div id="item2"></div><div id="item3"></div>
img[src="image$.jpg"]*3 → <img src="image1.jpg"><img src="image2.jpg"><img src="image3.jpg">
```

### Numbering modifiers
```
li.item$$$*3 → <li class="item001"></li><li class="item002"></li><li class="item003"></li>
li.item$@-*3 → <li class="item3"></li><li class="item2"></li><li class="item1"></li>
li.item$@3*3 → <li class="item3"></li><li class="item4"></li><li class="item5"></li>
```

### Text ({})
```
p{Hello World} → <p>Hello World</p>
div{Content $}*3 → <div>Content 1</div><div>Content 2</div><div>Content 3</div>
a{Click me} → <a href="">Click me</a>
```

### Common HTML5 Snippets
```
! → Complete HTML5 boilerplate
html:5 → HTML5 document structure
meta:vp → <meta name="viewport" content="width=device-width, initial-scale=1.0">
link:css → <link rel="stylesheet" href="style.css">
script:src → <script src=""></script>
```

### Form Elements
```
form → <form action=""></form>
input → <input type="text">
input:text → <input type="text" name="" id="">
input:email → <input type="email" name="" id="">
input:password → <input type="password" name="" id="">
input:submit → <input type="submit" value="">
select → <select name="" id=""></select>
option → <option value=""></option>
textarea → <textarea name="" id="" cols="30" rows="10"></textarea>
```

### Complex Examples
```
div.container>header.header>nav.navbar>ul.nav-list>li.nav-item*4>a.nav-link{Item $}

table.data-table>thead>tr>th*4{Header $}^^tbody>tr*3>td*4{Data $-$}

form.contact-form>(div.form-group>label{Name}+input:text)+(div.form-group>label{Email}+input:email)+button:submit{Send}
```

## CSS Syntax

### Properties
```
p → padding
m → margin
w → width
h → height
bg → background
c → color
fz → font-size
lh → line-height
ta → text-align
d → display
pos → position
```

### Values with Units
```
w100 → width: 100px
h50p → height: 50%
m10-20 → margin: 10px 20px
p10-15-20-25 → padding: 10px 15px 20px 25px
```

### Vendor Prefixes
```
-webkit-transform → -webkit-transform: ;
-moz-transform → -moz-transform: ;
-ms-transform → -ms-transform: ;
-o-transform → -o-transform: ;
```

### Common CSS Snippets
```
dn → display: none
db → display: block
dib → display: inline-block
df → display: flex
pr → position: relative
pa → position: absolute
pf → position: fixed
fl → float: left
fr → float: right
cl → clear: both
tac → text-align: center
tal → text-align: left
tar → text-align: right
```

### Flexbox
```
d:f → display: flex
fxd:c → flex-direction: column
fxw:w → flex-wrap: wrap
jc:c → justify-content: center
ai:c → align-items: center
as:c → align-self: center
```

### Colors
```
c:r → color: red
bg:b → background: blue
bg:#123 → background: #123
bg:rgba → background: rgba(0, 0, 0, 0)
```

### Borders
```
bd → border: 1px solid #000
bd+ → border: 1px solid #000
bdt → border-top: 1px solid #000
bdb → border-bottom: 1px solid #000
bdl → border-left: 1px solid #000
bdr → border-right: 1px solid #000
```

### Shortcuts for Common Patterns
```
! → !important
bg:n → background: none
c:t → color: transparent
op:0.5 → opacity: 0.5
zi:999 → z-index: 999
```

## Tips and Tricks

### Tab Expansion
- Type the abbreviation and press `Tab` to expand
- Works in most modern code editors (VS Code, Sublime Text, Atom, etc.)

### Custom Snippets
- Most editors allow you to create custom Emmet snippets
- Useful for frequently used code patterns in your projects

### Lorem Ipsum
```
lorem → Generates Lorem Ipsum text
lorem10 → Generates 10 words of Lorem Ipsum
lorem*3 → Generates 3 paragraphs of Lorem Ipsum
```

### Emmet in CSS
- Works inside `<style>` tags in HTML
- Available in separate CSS files
- Speeds up writing CSS properties and values

### Wrap with Abbreviation
- Select text in your editor
- Use "Wrap with Abbreviation" command
- Type Emmet abbreviation to wrap selected content

### Balance Tags
- Use Emmet's balance inward/outward commands
- Helps select matching HTML tags quickly
- Useful for navigation and editing

Remember: Emmet is case-insensitive and works with custom elements too!


----------------------------------------------------------------------------------------------
# Css Common used properties
1.Box Model
<img width="260" height="222" alt="image" src="https://github.com/user-attachments/assets/393279d1-cf53-4d7a-ba64-c152fb4546e6" />

2.Position Property
  1.Static 
  2.Relative
  3.Fixed
  4.Absolute
  4.Sticky
  
3.Flex box
<img width="267" height="357" alt="image" src="https://github.com/user-attachments/assets/f969cbdf-26e6-455c-9886-e58332cbfda0" />
<img width="978" height="388" alt="image" src="https://github.com/user-attachments/assets/3cf03be7-f29a-4358-9a68-dcfe34f4b210" />
looks like it applis the child of multiple niot on parent

4.grid property
<img width="528" height="137" alt="image" src="https://github.com/user-attachments/assets/b52e183b-ac99-4c63-84db-cf91aa3843b3" />


