# Sage math language support in Atom
Adds syntax highlighting and snippets to Sage math files in Atom. Currently limited to basic python syntax.

Originally forked from the atom.io [Python language bundle](https://github.com/atom/language-python), which was [converted](http://atom.io/docs/latest/converting-a-text-mate-bundle)
from the [Python TextMate bundle](https://github.com/textmate/python.tmbundle).

To fix `in,is,not,and,or` and parameters for functions being highlighted, add the following to your personal stylesheet (which can be found at Packages -> Settings View -> Manage Themes -> _your stylesheet_):
```
// To style other content in the text editor's shadow DOM, use the ::shadow expression
atom-text-editor::shadow {
  // Add Your Styles Here
  .keyword.operator.logical.sage { color: #c678dd; }
  .variable.parameter { color: hsl( 29, 54%, 61%); }
}
```
Customize those two colors according to your preferred theme, the given two colors are the colors for the one-dark-syntax theme by atom.

Contributions are greatly appreciated. Please fork this repository and open a
pull request to add snippets, make grammar tweaks, etc.
