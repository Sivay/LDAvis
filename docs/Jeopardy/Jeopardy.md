Jeopardy Data
==============

[Click here](http://cpsievert.github.io/LDAvis/Jeopardy/vis) to see the result of the code below:


```r
library("LDAvis")
data(Jeopardy, package = "LDAvisData")
json <- with(Jeopardy, createJSON(phi, theta, doc.length, vocab, term.frequency))
serVis(json, out.dir = 'vis', open.browser = FALSE)
```
