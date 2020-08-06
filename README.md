# Web Workers
# miből lesz a cserebogár
#  Cli ből küldött pull-request 

You can run highlighting inside a web worker to avoid freezing the browser window while dealing with very big
chunks of code.

In your main script:

```javascript
addEventListener("load", () => {
  const code = document.querySelector("#code");
  const worker = new Worker("worker.js");
  worker.onmessage = event => {
    code.innerHTML = event.data;
  };
  worker.postMessage(code.textContent);
});
```

In worker.js:

```javascript
onmessage = event => {
  importScripts("<path>/highlight.min.js");
  const result = self.hljs.highlightAuto(event.data);
  postMessage(result.value);
};
```

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

![Image of professorcat](https://arajczy.duckdns.org/images/cat.png)

```javascript
if (isAwesome) {
  return true;
}
```

Here is a footnote reference,[^1] and another.[^longnote]

[^1]: Here is the footnote.
[^longnote]: Here's one with multiple blocks.

  Subsequent paragraphs are indented to show that they

belong to the previous footnote.

- [x] This is a complete item
- [ ] This is an incomplete item

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

Here is an inline note.^[Inlines notes are easier to write, since
you don't have to pick an identifier and move down to type the
note.]

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

:+1: :-1: :x:

---

:smile: :disappointed: :rage:

---

:tada: :palm_tree: :hamburger:

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/M6dXXPhk-3I/0.jpg)](https://www.youtube.com/watch?v=M6dXXPhk-3I)

http://github.com - automatic!
[GitHub](http://github.com)
