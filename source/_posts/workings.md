---
layout: page
title: mermaid and math workings test...
description: >
hide_description: false
---

## 0

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
click D href "https://google.com"
```
<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
click D href "https://google.com"
</div>

## 1

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

|--|--|--|--|--|--|--|--|
|♜| |♝|♛|♚|♝|♞|♜|
| |♟|♟|♟| |♟|♟|♟|
|♟| |♞| | | | | |
| |♗| | |♟| | | |
| | | | |♙| | | |
| | | | | |♘| | |
|♙|♙|♙|♙| |♙|♙|♙|
|♖|♘|♗|♕|♔| | |♖|

## 2

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<div class="markdown">
|--|--|--|--|--|--|--|--|
|♜| |♝|♛|♚|♝|♞|♜|
| |♟|♟|♟| |♟|♟|♟|
|♟| |♞| | | | | |
| |♗| | |♟| | | |
| | | | |♙| | | |
| | | | | |♘| | |
|♙|♙|♙|♙| |♙|♙|♙|
|♖|♘|♗|♕|♔| | |♖|
</div>  


## 3

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<div class="mermaid">
gantt;
[Prototype design] lasts 15 days
[Test prototype] lasts 10 days
-- All example --
[Task 1 (1 day)] lasts 1 day
[T2 (5 days)] lasts 5 days
[T3 (1 week)] lasts 1 week
[T4 (1 week and 4 days)] lasts 1 week and 4 days
[T5 (2 weeks)] lasts 2 weeks
</div>

## 4

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

[Prototype design] lasts 15 days
[Test prototype] lasts 10 days
-- All example --
[Task 1 (1 day)] lasts 1 day
[T2 (5 days)] lasts 5 days
[T3 (1 week)] lasts 1 week
[T4 (1 week and 4 days)] lasts 1 week and 4 days
[T5 (2 weeks)] lasts 2 weeks

## 5

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<div class="mermaid">
graph TD;
A[Client] --> B[Load Balancer] 
B --> C[Server01] 
B --> D[Server02]
</div>

@startmermaid
graph TD;
A[Client] --> B[Load Balancer] 
B --> C[Server01] 
B --> D[Server02]
@endmermaid



## 6
- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
</div>



## 7 IAL

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not


|:             Here's an Inline Attribute Lists example                :||||
| ------- | ------------------ | -------------------- | ------------------ |
|:       :|:  <div style="color: red;"> &lt; Normal HTML Block > </div> :|||
| ^^      |   Red    {: .cls style="background: orange" }                |||
| ^^ IALs |   Green  {: #id style="background: green; color: white" }    |||
| ^^      |   Blue   {: style="background: blue; color: white" }         |||
| ^^      |   Black  {: color-style text-style }                         |||


## 8

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not

| :        Fruits \|\| Food       : |||
| :--------- | :-------- | :--------  |
| Apple      | : Apple : | Apple      \
| Banana     |   Banana  | Banana     \
| Orange     |   Orange  | Orange     |
| :   Rowspan is 4    : || How's it?  |
|^^    A. Peach         ||   1. Fine :|
|^^    B. Orange        ||^^ 2. Bad   |
|^^    C. Banana        ||  It's OK!  |

## 9

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not

| :                    MathJax \|\| Image                 : |||
| :------------ | :-------- | :----------------------------- |
| Apple         | : Apple : | Apple                          \
| Banana        | Banana    | Banana                         \
| Orange        | Orange    | Orange                         |
| :     Rowspan is 4     : || :        How's it?           : |
| ^^     A. Peach          ||    1. ![example][cell-image]   |
| ^^     B. Orange         || ^^ 2. $I = \int \rho R^{2} dV$ |
| ^^     C. Banana         || **It's OK!**                   |

[cell-image]: https://jekyllrb.com/img/octojekyll.png "An exemplary image"

## 10

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not

$I = \int \rho R^{2} dV$  
$ 3 * 3 $

<a href="http://www.google.com">여기를 클릭</a>


## 11

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not


<div class="mermaid">
gantt
    dateFormat  YYYY-MM-DD
    title       Adding GANTT diagram functionality to mermaid
    excludes    weekends
    %% (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)

    section A section
    Completed task            :done,    des1, 2014-01-06,2014-01-08
    Active task               :active,  des2, 2014-01-09, 3d
    Future task               :         des3, after des2, 5d
    Future task2              :         des4, after des3, 5d

    section Critical tasks
    Completed task in the critical line :crit, done, 2014-01-06,24h
    Implement parser and jison          :crit, done, after des1, 2d
    Create tests for parser             :crit, active, 3d
    Future task in critical line        :crit, 5d
    Create tests for renderer           :2d
    Add to mermaid                      :1d
    Functionality added                 :milestone, 2014-01-25, 0d

    section Documentation
    Describe gantt syntax               :active, a1, after des1, 3d
    Add gantt diagram to demo page      :after a1  , 20h
    Add another diagram to demo page    :doc1, after a1  , 48h

    section Last section
    Describe gantt syntax               :after doc1, 3d
    Add gantt diagram to demo page      :20h
    Add another diagram to demo page    :48h
</div>

## 12

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
<blockquote class="twitter-tweet" data-lang="en">
  <p lang="en" dir="ltr">
    The next version of Hydejack (v6.3.0) will allow embedding 3rd party scripts,
    like the one that comes with this tweet for example.
  </p>
  &mdash; Florian Klampfer (@qwtel)
  <a href="https://twitter.com/qwtel/status/871098943505039362">June 3, 2017</a>
</blockquote>

  


## 13

- [x] rendered on VS code preview or not
- [ ] renderd on built site or not

<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
click D href "https://google.com"
</div>


## 14

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not

$$
a * b = c ^ b   \\
2^{\frac{n-1}{3}}  \\  
\int\_a^b f(x)\,dx.  \\
$$

-------------------
$$
\begin{aligned} %!!15
  \phi(x,y) &= \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right) \\[2em]
            &= \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j)            \\[2em]
            &= (x_1, \ldots, x_n)
               \left(\begin{array}{ccc}
                 \phi(e_1, e_1)  & \cdots & \phi(e_1, e_n) \\
                 \vdots          & \ddots & \vdots         \\
                 \phi(e_n, e_1)  & \cdots & \phi(e_n, e_n)
               \end{array}\right)
               \left(\begin{array}{c}
                 y_1    \\
                 \vdots \\
                 y_n
               \end{array}\right) \\
\end{aligned}
$$

## 15
- maermaidjs live editor.

- [o] rendered on VS code preview or not
- [ ] renderd on built site or not

[![](https://mermaid.ink/img/pako:eNplj7EOwjAMRH_F8twFIZasFDF1Yu1iNRY10BiljqoK8e-klEoFMiXvznfOAxv1jA4BLppi4LEOkI-J3RiqEQaNVwln8PRRem5MNMBRwfQtzxygoiuDMTnYOah4wdmY7r2RxN7Bdq2U87yDzUQL2JP9dbTarZO8DmHJ-mo5ib3FnwossOPYkfj8x8dEa7SWcya6fPWU18c6PLMv3T0ZH7yYRnQWExdIyfQ0hmZ5z55S6Bypm-HzBR-_ZCw)](https://mermaid-js.github.io/mermaid-live-editor/edit#pako:eNplj7EOwjAMRH_F8twFIZasFDF1Yu1iNRY10BiljqoK8e-klEoFMiXvznfOAxv1jA4BLppi4LEOkI-J3RiqEQaNVwln8PRRem5MNMBRwfQtzxygoiuDMTnYOah4wdmY7r2RxN7Bdq2U87yDzUQL2JP9dbTarZO8DmHJ-mo5ib3FnwossOPYkfj8x8dEa7SWcya6fPWU18c6PLMv3T0ZH7yYRnQWExdIyfQ0hmZ5z55S6Bypm-HzBR-_ZCw)


## 16



<svg viewBox="0 0 1904 450" aria-labelledby="chart-title-mermaid-svg chart-desc-mermaid-svg" role="img" style="max-width: 1904px;" height="450" xmlns="http://www.w3.org/2000/svg" width="100%" id="mermaid-svg"><title id="chart-title-mermaid-svg">Pets adopted by volunteers</title><desc id="chart-desc-mermaid-svg"></desc><style>#mermaid-svg {font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#333;}#mermaid-svg .error-icon{fill:#552222;}#mermaid-svg .error-text{fill:#552222;stroke:#552222;}#mermaid-svg .edge-thickness-normal{stroke-width:2px;}#mermaid-svg .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg .marker{fill:#333333;stroke:#333333;}#mermaid-svg .marker.cross{stroke:#333333;}#mermaid-svg svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg .pieCircle{stroke:black;stroke-width:2px;opacity:0.7;}#mermaid-svg .pieTitleText{text-anchor:middle;font-size:25px;fill:black;font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg .slice{font-family:"trebuchet ms",verdana,arial,sans-serif;fill:#333;font-size:17px;}#mermaid-svg .legend text{fill:black;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:17px;}#mermaid-svg :root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}</style><g></g><g transform="translate(952,225)"><path class="pieCircle" fill="#ECECFF" d="M1.1327982892113017e-14,-185A185,185,0,1,1,-177.89919060802214,-50.76295874957067L0,0Z"></path><path class="pieCircle" fill="#ffffde" d="M-177.89919060802214,-50.76295874957067A185,185,0,0,1,-35.651768201396706,-181.53223246606615L0,0Z"></path><path class="pieCircle" fill="hsl(80, 100%, 56.2745098039%)" d="M-35.651768201396706,-181.53223246606615A185,185,0,0,1,-1.982969563208622e-13,-185L0,0Z"></path><text style="text-anchor: middle;" class="slice" transform="translate(55.715631369627125,73.83778450823009)">79%</text><text style="text-anchor: middle;" class="slice" transform="translate(-62.60222388060678,-68.09707457154371)">17%</text><text style="text-anchor: middle;" class="slice" transform="translate(-8.955005540044146,-92.06550861086782)">3%</text><text class="pieTitleText" y="-200" x="0">Pets adopted by volunteers</text><g transform="translate(216,-33)" class="legend"><rect style="fill: rgb(236, 236, 255); stroke: rgb(236, 236, 255);" height="18" width="18"></rect><text y="14" x="22">Dogs</text></g><g transform="translate(216,-11)" class="legend"><rect style="fill: rgb(255, 255, 222); stroke: rgb(255, 255, 222);" height="18" width="18"></rect><text y="14" x="22">Cats</text></g><g transform="translate(216,11)" class="legend"><rect style="fill: rgb(181, 255, 32); stroke: rgb(181, 255, 32);" height="18" width="18"></rect><text y="14" x="22">Rats</text></g></g><style>@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css");</style></svg>)


## 17

<div class="mermaid">
graph TD;
    A[Loading URL failed. We can try to figure out why.] -->|Decode JSON| B(Please check the console to see the JSON and error details.)
    B --> C{Is the JSON correct?}
    C -->|Yes| D(Please Click here to Raise an issue in github.<br/>Including the broken link in the issue <br/> will speed up the fix.)
    C -->|No| E{Did someone <br/>send you this link?}
    E -->|Yes| F[Ask them to send <br/>you the complete link]
    E -->|No| G{Did you copy <br/> the complete URL?}
    G --> |Yes| D
    G --> |"No :("| H(Try using the Timeline tab in History <br/>from same browser you used to create the diagram.)
    click D href "https://github.com/mermaid-js/mermaid-live-editor/issues/new?assignees=&labels=bug&template=bug_report.md&title=Broken%20link" "Raise issue"
</div>

## 18 

@startuml
object Object01
object Object02
object Object03
object Object04
object Object05
object Object06
object Object07
object Object08

Object01 <|-- Object02
Object03 *-- Object04
Object05 o-- "4" Object06
Object07 .. Object08 : some labels
@enduml

## 19

@startmermaid
gantt;
[Prototype design] lasts 15 days
[Test prototype] lasts 10 days
-- All example --
[Task 1 (1 day)] lasts 1 day
[T2 (5 days)] lasts 5 days
[T3 (1 week)] lasts 1 week
[T4 (1 week and 4 days)] lasts 1 week and 4 days
[T5 (2 weeks)] lasts 2 weeks
@endmermaid


## 20

[Alt text](./mermaid1.svg)

## 21

<img src="./mermaid1.svg">

## 22

[Alt text](./mermaid2.svg)
