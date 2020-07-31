# my first repository

It's very easy to make some words **bold** and other words _italic_ or ~~striked~~ with Markdown. You can even [Link to Google!](http://google.com)

Sometimes you want numbered lists:

1. One
1. Two
1. Three

Sometimes you want bullet points:

- Start a line with a star
- Profit!

If you want to embed images, this is how you do it:

![Image of professorcat](https://mysite.github.com/images/cat.png)

```javascript
if (isAwesome) {
  return true;
}
```

- [x] This is a complete item
- [ ] This is an incomplete item

| First Header | Second Header |
| ------------ | ------------- |
| Cell 1       | Cell 2        |
| Cell A       | Cell B        |

Colons can be used to align columns.

| Tables        |      Are      |   Cool |
| ------------- | :-----------: | -----: |
| col 3 is      | right-aligned | \$1600 |
| col 2 is      |   centered    |   \$12 |
| zebra stripes |   are neat    |    \$1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          |

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

:+1: :-1:

---

:smile: :disappointed: :rage:

---

:tada: :tree: :coctail:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/=M6dXXPhk-3I/0.jpg)](https://www.youtube.com/watch?v=M6dXXPhk-3I)

``` flowchart
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End|future:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|future

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```
