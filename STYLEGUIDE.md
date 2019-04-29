portfolio-src
=================

Style guide for my portfolio project.

**Note:** You have to install `kss-node` at first.

How to apply this style guide?
------------------------------
1. Install kss-node. Type `npm install kss` or `npm install -g kss` for global CLI.
2. Run `kss` command.

```
kss --source <sourcedir> --homepage <homepage> --title <title>
```


TL:DR;
===================

Format
------
kss-node is almost compatible with KSS documentation.
But kss-node can depend on only comment in source code because it has `Markup:` directive for showing the sample markup.

Here is a basic format for kss-node documentation.

```css
/*
Buttons

A majority of buttons in the site are built from the same base class.

:hovered    - Highlight the button when hovered.
:disabled   - Make the button change appearance to reflect it being disabled.
.primary    - Indicate that the button is the primary feature of this form.

Markup:
<a href="#" class="button {{modifier_class}}">Link Button</a>
<button class="button {{modifier_class}}">Button Element</button>

Styleguide 1.1
*/
.button {
  ...
}
.button:hover {
  ...
}
.button:disabled {
  ...
}
.button.primary {
  ...
}
```

As you see in the above samples, kss-node comment has some blocks.
From the top,

1. Element's title
2. Element's description
3. List of modifier classes or pseudo-classes
4. HTML markup
5. Reference to the element's position in the styleguide

And each description supports the Markdown writing.
