<!--

author: André Dietrich

script:   https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.3.1/papaparse.min.js

@CSV
<script style="display:block" run-once modify="false">
let url = "@0"

Papa.parse(url, {
  download: true,
  complete: function(r){
    let str = "|"
    let sep = "|"

    for(let i=0; i<r["data"][0].length; i++) {
      str += " " + r["data"][0][i] + " |"
      sep += "---|"
    }
    str += "\n"+ sep

    for(let i=1; i<r.data.length -1; i++) {
      str +="\n|"
      for(let j=0; j<r["data"][i].length; j++) {
        str += " " + r["data"][i][j] + " |"
      }
    }
    send.liascript(str)
  }
})

send.liascript("loading: " + url)
</script>
@end

-->

# Custom extensions



## Macros

<div style="width:100%;height:0;padding-bottom:100%;position:relative;"><iframe src="https://giphy.com/embed/Y4UvJMJSdA5qWir7Bh" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/Keto-Mojo-keto-fasting-ketones-Y4UvJMJSdA5qWir7Bh">via GIPHY</a></p>


### Single Line:
<!--
author: SOmeOne Else
-->

@author








### Parameters `@0` ... `@9`
<!--
@highlight: <span style="color: @0">@1</span>
-->

_@highlight(green, this is shall be red)_

@highlight(#F00, __BUT THIS TIME__ it is red)






### Multi Line `... @end`
<!--

@img: <img alt="@0" src="https://creativecommons.org/images/deed/@1" style="height: 40px">


@LICENSE
> @img(cc logo,cc_icon_white_x2.png) @img(cc pd,zero_white_x2.png)
>
> ## CC0 1.0 Universal (CC0 1.0)
>
>  The person who associated a work with this deed has dedicated the work to the public domain by waiving all of his or her rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law.
>
>You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission.
@end

-->


@LICENSE








## JavaScript


!?[Media for Thinking the Unthinkable](https://www.youtube.com/watch?v=oUaOucZRlmE "Bret Victor on data-driven publishing")




### Starting simple

<script>2**4</script>



### Combining scripts

<script input="range" default="2" output="x">
@input
</script>
to the power of 2 is
<script>
@input(`x`) ** 2
</script>



### Combining JS & Macros
<!--
pow: <script>@0 ** @input(`n`)</script>
-->

<script input="range" default="0" output="n">
@input
</script>

<!-- data-type="line" -->
| x |   x^n   |
|---|---------|
| 1 | @pow(1) |
| 2 | @pow(2) | 
| 3 | @pow(3) |
| 4 | @pow(4) |
| 5 | @pow(5) |
| 6 | @pow(6) |
| 7 | @pow(7) |
| 8 | @pow(8) |



### Reducing Complexity

@CSV(https://raw.githubusercontent.com/arcus/LIEAF2022_workshop/main/data/health_expenditure.csv)

@[CSV](https://raw.githubusercontent.com/arcus/LIEAF2022_workshop/main/data/health_expenditure.csv)

## Where to find extensions

[here](https://github.com/topics/liascript-template)


# lightweight - ClassRoom

What is $2^4$?

[( )] 2
[( )] 4
[( )] 8
[(X)] 16

---

Rate this presentation?

[(5)] Far exceeded my expectations.
[(4)] Exceeded my expectations.
[(3)] Met my expectations.
[(2)] I’d expected more.
[(1)] Way below my expectations.

---

Do you have any questions?

[[___ ___]]


