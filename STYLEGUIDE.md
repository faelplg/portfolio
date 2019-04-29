Portfolio style guide
=========================

How it works?
------------------------------
1. Install `kss-node`. Type `npm install kss`.
2. Install `npx`.
2. Run the command:

```
npx kss --source <sourcedir> --homepage <homepage> --title <title>
```

TL:DR;
-------------

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

As you see in the above samples, `kss-node` comment has some blocks.
From the top,

1. Element's title
2. Element's description
3. List of modifier classes or pseudo-classes
4. HTML markup
5. Reference to the element's position in the style guide

And each description supports the Markdown writing.
