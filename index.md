# Textarea Editor
An extensible editor which, at its core, is an HTML `<textarea>` (hence the name) and responsive panels, and browser JavaScript modules to add real functionality to it.

**[Begin Editing](editor.html)**

The editor is fully self-contained, so you can easily download the file and work offline. The editor relies on nothing external, so you don't have to worry about privacy. Modules can still be ignorant of privacy, however, and can be dangerous. So be sure to pick modules that you can *trust*.

## I only see a textarea
The link is to the Textarea Editor *core*. You need to add *modules* to it to make it more functional.

Modules are in browser JavaScript, and can be imported by adding `<script>` elements to the editor document.

## When I quit the page, I lose the contents of the textarea
The textarea doesn't have magic abilities of keeping data. You need to use modules for saving.

## Okay, how do I make modules?
You just need browser JavaScript.

Modules can refer to any of the six main parts of the editor:
- the side bar (`#sidebar`), for keeping forms;
- the tool bar (`#toolbar`), for adding action buttons;
- the tab bar (`#tabbar`), for interacting with multiple files;
- the project bar (`#projectbar`), for keeping forms related to a project;
- the status bar (`#statusbar`), for keeping stats in a concise form; and
- the textarea itself (`#textarea`), for reading and writing text in the textarea.

The Textarea Editor doesn't export anything else.

Lastly, you need to publish it somewhere from where it can be imported by adding a `<script>` element to the editor document.
