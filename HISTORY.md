# DocBlockr Extended Changelog

- **v2.14.1**, *17 Aug 2015*
  - Fix deindentation bug with reparsing doc blocks
- **v2.14.0**, *15 Jun 2015*
  - Adds `jsdocs_function_description` option (thanks to [Gerard Roche](https://github.com/gerardroche))
  - Better handling of parser errors (thanks to Gerard Roche)
- **v2.13.3**, *4 Jun 2015*
  - PHP array shorthand is identified correctly (thanks to [Gerard Roche](https://github.com/gerardroche))
  - Decorating comments when using tabs for indentation works better (thanks to [Jack Cherng](https://github.com/jfcherng))
- **v2.13.2**, *30 Mar 2015*
  - Updated PHPDoc autocompletions to align with the new spec (thanks to [Gerard Roche](https://github.com/gerardroche))
  - Properly handle the case when commas appear inside a type name in Java
  - Added link to README in the preferences menu
- **v2.13.1**, *29 Mar 2015*
  - Adds support for Apex language (thanks @michacom)
  - Fixes identifying multidimensional arrays in C/C++
  - Fixes reformatting and reparsing docblocks in Java
  - Adds options to disable:
    - opening an inline docblock with space (`jsdocs_quick_open_inline`)
    - inline comment decoration (`jsdocs_decorate`)
- **v2.13.0**, *11 Dec 2014*
  - ECMAScript 6 support! Including:
    - Arrow functions
    - Default parameter values
    - Rest parameters
    - Parameter destructuring
    - Shorthand method initialization
    - `@yield` for generator functions
- **v2.12.4**, *10 Dec 2014*
  - Fixes regression in handling Javascript function expressions
- **v2.12.3**, *7 Dec 2014*
  - PHP arguments with pass-by-reference handled properly, thanks to [Gerard Roche](https://github.com/gerardroche)
  - PHP namespaces handled properly, thanks to Gerard Roche
  - PHP parameters with default null values handled properly, thanks to Gerard Roche
  - ECMAScript 6 generator functions handled properly, thanks to [Sergey Zarouski](https://github.com/szarouski)
  - Parameter name can be omitted with `jsdocs_param_name` option, thanks to [Daniel Kurecka](https://github.com/danielkurecka)
  - Inline docblocks are expanded with <kbd>space</kbd>, thanks to Daniel Kurecka
  - Java array types handled properly, thanks to [Alessio Linares](https://github.com/Galbar)
- **v2.12.2**, *11 Apr 2014*
  - Fix for PHP autocompletions
  - Fix `@name` completion for Javascript
- **v2.12.1**, *4 Mar 2014*
  - Fix for Sublime Text 3
- **v2.12.0**, *4 Mar 2014*
  - Adds support for **TypeScript**, thanks to [Marc-Antoine Parent](https://github.com/maparent)
  - Adds option to add a spacer line after the description (`"jsdocs_spacer_between_sections": "after_description"`), thanks to [Milos Levacic](https://github.com/levacic)
  - PHP autocompletions support only the [PSR-5](https://github.com/phpDocumentor/fig-standards/blob/master/proposed/phpdoc.md) tags, thanks to [Gary Jones](https://github.com/GaryJones)
  - Fix scope issues for Java autocompletions, thanks to [Dominique Wahli](https://github.com/bizoo)
  - Fix for reflowing paragraphs when no rulers are set.
- **v2.11.7**, *3 Nov 2013*
  - Added support for triple `///`, `//!` and `/*!` style comments, thanks to [Jordi Boggiano](https://github.com/seldaek).
  - Added basic **Rust** support, again thanks to Jordi Boggiano.
  - Added an option to use short names for bools and ints (`jsdocs_short_primitives`), thanks to [Mat Gadd](https://github.com/drarok).
  - Fixed a bug with per-section indenting, again thanks to Mat Gadd.
  - Improved handling of Java return type detection, thanks to [Ben Linskey](https://github.com/blinskey)
- **v2.11.6**, *14 Aug 2013*
  - Predefined `@author` tags do not get parsed for column spacing
  - Handles the case when an arguments list contains a comma, for example, within a default value
  - A new keybinding for Windows to re-parse a doc block (<kbd>Alt+W</kbd>)
  - Fixes a regression that some function names were not being parsed correctly
- **v2.11.5**, *11 Aug 2013*
  - Fix for last deploy which accidentally changed the default `var` tag to "property". Default is "type" once again.
- **v2.11.4**, *10 Aug 2013*
  - The tag used on `var` declarations can be customised (eg: to "property" for YUIDoc)
  - Small fix for function declarations in C/C++ (thanks to [Simon Aittamaa](https://github.com/simait))
- **v2.11.3**, *18 June 2013*
  - Adds support for Groovy (thanks to [Tiago Santos](https://github.com/tmcsantos))
  - README has gifs. So many gifs.
- **v2.11.2**, *12 June 2013*
  - Compatibility fixes for ST3, thanks to Marc Neuhaus (@mneuhaus) and Daniel Julius Lasiman (@danieljl).
- **v2.11.1**, *11 May 2013*
  - No changes, just removes some debugging code that wasn't cleaned up in the last release (oops).
- **v2.11.0**, *11 May 2013*
  - It isn't broken in ST3 any more. (yay)
  - New options:
    - `jsdocs_simple_mode` for when you don't want dynamic templates
    - `jsdocs_lower_case_primitives` for YUIDoc which requires lower case for primitive data types
    - `jsdocs_extra_tags_go_after` to put custom text at the end of the docblock
  - Better handling of IIFEs
  - Hotkey for reparsing a block changed to <kbd>alt+shift+tab</kbd> to avoid OS-level conflicts
  - Adding a new line at the start of the docblock is handled properly
  - C/C++: arguments containing square brackets are handled properly
- **v2.10.1**, *19 April 2013*
  - Adds variable substitution in `jsdocs_extra_tags`
  - Fixes indentation bug in `jsdocs_extra_tags`
  - Fixes bug when adding a new line after a docblock which contains text afterwards
  - Fixes link to Pledgie (thanks @Krinkle)
- **v2.10.0**, *21 February 2013*
  - Adds Sublime Text 3 support (thanks to @lxe and @rmarscher)
  - YUI-style `@method` tags can be automatically added with the `jsdocs_autoadd_method_tag` setting (thanks to @maheshjag)
  - Variables starting with `$` are not wiped out when reparsing a doc block (thanks @ryrun)
- **v2.9.3**, *12 December 2012*
  - Fixed bug which stopped regular comments from closing automatically
- **v2.9.2**, *11 December 2012*
  - This one goes out to [Thanasis Polychronakis](https://github.com/thanpolas).
    - Structure of the modules greatly improved
    - Fixes bug with matching languages with hyphens in the name
  - Adds support for CUDA-C++
- **v2.9.1**, *31 October 2012*
  - Thanks to [wronex](https://github.com/wronex), <kbd>Alt+Q</kbd> will reformat the entire DocBlock, with customisable indentation.
  - Thanks to [Pavel Voronin](https://github.com/pavel-voronin), spaces around arguments are handled properly.
  - **C/C++**: Array arguments are accepted
  - **C/C++**: An argument list containing only `void` doesn't output any `@param` tags
  - **PHP**: Arguments with an array as a default value inside multi-line arguments are handled properly
  - <kbd>Ctrl/Cmd + Enter</kbd> and <kbd>Ctrl/Cmd + Shift + Enter</kbd> work inside DocBlocks.
- **v2.9.0**, *1 October 2012*
  - Adds ObjectiveC and ObjectiveC++ support, thanks to some help from [Robb B??hnke](https://github.com/robb)
    - Very buggy code, support isn't great but it's better than nothing (hopefully).
  - Single-line comments inside function definitions are handled
  - Notation rules are applied to functions, which means they can define a return type by their name, eg: `strFoo`
  - Notation rules can define arbitrary tags, for example: functions with a prefix of "_" should get the `@private` tag.
  - Given the above addition, JS functions starting with an underscore are no longer marked as `@private` by default.
- **v2.8.2**, *28 September 2012*
  - When a function is defined across many lines, the parser will find the arguments on extra lines.
- **v2.8.1**, *13 September 2012*
  - Pressing <kbd>tab</kbd> on an empty line will perform a deep indentation instead of moving to the next field
  - Functions starting with `_` will get a `@private` tag in Javascript (thanks to [Andrew Hanna](https://github.com/percyhanna))
- **v2.8.0**, *26 August 2012*
  - New feature: <kbd>Alt+Q</kbd> to reformat the description field of a docblock to make it fit nicely within your ruler.
  - Adds support for C++ (thanks to [Rafa?? Ch??odnicki](https://github.com/rchl))
  - Indenting to the description field works in languages which don't require type information in the docblock.
- **v2.7.4**, *8 August 2012*
  - Fix for Actionscript docblocks not working
- **v2.7.3**, *7 August 2012*
  - No trailing whitespace added on the spacer lines added when `jsdocs_spacer_between_sections` is on (thanks to [Rafa?? Ch??odnicki](https://github.com/rchl))
  - Fixes a bug with detecting variable names when they have a default value in PHP
  - Changes the notation map to not ignore the leading `$` or `_`, meaning that (for example), you could specify that variables starting with `$` are `HTMLElement`s.
- **v2.7.2**, *6 August 2012*
  - Small bug fix, thanks to [djuliusl](https://github.com/djuliusl)
- **v2.7.1**, *5 August 2012*
  - Adds per-section alignment (can be set using `jsdocs_per_section_indent`)
  - Description field for `@return` tag can be disabled using `jsdocs_return_description`. *(Both thanks to [Drarok](https://github.com/Drarok))*
- **v2.7.0**, *5 August 2012*
  - Adds support for ASDocs (Actionscript)
  - Changes Linux shortcut for reparsing a comment block to <kbd>Alt+Shift+Tab</kbd>
- **v2.6.5**, *19 June 2012*
  - Bugfix for adding linebreaks when not at the start or end of a line
- **v2.6.4**, *4 June 2012*
  - Better support for indentation using tabs
  - YUI tags are supported by the autocomplete
  - When only whitespace exists on a docblock line, and `trim_automatic_white_space` is set to true, the whitespace is removed.
  - Better support for comment blocks opened with `/*`
- **v2.6.3**, *30 April 2012*
  - Fixes the join-lines command <kbd>Ctrl+J</kbd> for CoffeeScript.
- **v2.6.2**, *22 March 2012*
  - PHP `__destruct` functions don't get a return value *(thanks to [Alex Whitman](https://github.com/whitman))*.
- **v2.6.1**, *16 March 2012*
  - Fixes bug whereby the return values of functions which are named `set` or `add`, *etc* were not being guessed correctly.
  - `@return` tags are now given a description field *(thanks to [Nick Dowdell](https://github.com/mikulad13))*.
- **v2.6.0**, *4 March 2012*
  - Added CoffeeScript support
- **v2.5.0**, *11 February 2012*
  - Implemented DocBlock reparsing to re-enable tabstop fields. Hotkey is `Ctrl+Alt+Tab`.
- **v2.4.1**, *2 February 2012*
  - Fixed bug [#36](https://github.com/spadgos/sublime-jsdocs/issues/36) whereby docblocks were not being properly extended inside of `<script>` tags in a HTML document.
- **v2.4.0**, *29 January 2012*
  - `Enter` at the end of a comment block (ie: after the closing `*/`) will insert a newline and de-indent by one space.
- **v2.3.0**, *15 January 2012*
  - `Ctrl+Enter` on a double-slash comment will now decorate that comment.
  - Added a setting (`jsdocs_spacer_between_sections`) to add spacer lines between sections of a docblock.
- **v2.2.2**, *12 January 2012*
  - Separated JS and PHP completions files. PHP completions don't have brackets around type information any more.
  - PHP now uses `@var` (instead of `@type`) for documenting variable declarations.
  - *Both of these changes are thanks to [svenax][svenax]*
- **v2.2.1**, *11 January 2012*
  - DocBlocks can be triggered by pressing `tab` after `/**`
  - Some bugfixes due to auto-complete changes in Sublime Text.
  - Fixed bug where indenting would not work on the first line of a comment.
- **v2.2.0**, *5 January 2012*
  - A configuration option can be set so that either `@return` or `@returns` is used in your documentation.
  - Language-specific tags now will only show for that language (eg: PHP has no `@interface` tag).
- **v2.1.3**, *31 December 2011*
  - Changed path for macro file to point to `Packages/DocBlockr`. If you are having issues, make sure that the plugin is installed in that location (**not** the previous location `Packages/JSDocs`).
- **v2.1.2**, *31 December 2011*
  - Renamed from *JSDocs* to *DocBlockr*, since it now does more than just Javascript.
- **v2.1.1**, *23 November 2011*
  - Fixed bug which broke the completions list
- **v2.1.0**, *19 November 2011*
  - Added a command to join lines inside a docblock which is smart to leading asterisks
  - Variable types are guessed from their name. `is` and `has` are assumed to be Booleans, and `callback`, `cb`, `done`, `fn` and `next` are assumed to be Functions.
  - You can now define your own patterns for mapping a variable name to a type.
  - Autocomplete works better now. `@` will also insert the "@" character, allowing you to add any tag you like, even if it isn't in the autocomplete list.
  - Added the full set of [PHPDoc][phpdoc] tags.
- **v2.0.0**, *6 November 2011*
  - PHP support added!
  - (Almost) complete rewrite to allow for any new languages to be added easily
    - *Please send feature requests or pull requests for new languages you'd like to add*
  - More options for aligning tags
- **v1.3.0**, *5 November 2011*
  - Improvements to handling of single-line comments
  - Functions beginning with `is` or `has` are assumed to return Booleans
  - Consolidated settings files into `Base File.sublime-settings`. **If you had configured your settings in `jsdocs.sublime-settings`, please move them to the Base File settings.**
  - Setting `jsdocs_extend_double_slashes` controls whether single-line comments are extended.
  - Pressing `tab` in a docblock will tab to match the description block of the previous tag. Use `jsdocs_deep_indent` to toggle this behaviour.
- **v1.2.0**, *6 October 2011*
  - Variable declarations can be documented. `Shift+enter` to make these inline
  - Double slash comments (`// like this`) are extended when `enter` is pressed
  - Class definitions detected and treated slightly differently (no return values pre-filled)
- **v1.1.0**, *3 October 2011*
  - DocBlockr parses the line following the comment to automatically prefill some documentation for you.
  - Settings available via menu
- **v1.0.0**, *28 September 2011*
  - Initial release
  - Comments are automatically closed, extended and indented.
