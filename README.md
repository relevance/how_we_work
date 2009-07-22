# Working on This Site

1. Start Jekyll with `jekyll --auto --server`, and Jekyll will notice
   when you've changed a file and regenerate it automatically.
1. Markdown allows HTML markup, but doesn't process Markdown within HTML tags.
   So try to avoid direct use of HTML tags if possible.
   That brings us to:
1. The default Markdown engine for Jekyll is Maruku.
   Maruku supports some widely used extensions to Markdown known as "PHP Markdown Extra."
   Plus, it supports some extensions of its own.
   Unfortunately, each of those things documents its extensions,
   rather than the complete augmented Markdown syntax.
   So to understand the complete syntax that Maruku supports, you must read:
   * John Gruber's original [Markdown](http://daringfireball.net/projects/markdown/syntax)
   * Plus [PHP Markdown Extra](http://michelf.com/projects/php-markdown/extra/)
   * Plus [Maruku's own extensions](http://maruku.rubyforge.org/maruku.html) 
1. If you have the Maruku gem installed, and the Maruku TextMate bundle,
   Control-Option-Command-P pops up a preview window of the generated HTML.
1. Please put each sentence on a separate line.
   If you have long sentences, it might make sense to make some clauses their own lines as well.
   This takes some getting used to,
   but it's much easier to make sense of diffs and revisions as the documents evolve.
   It also makes it easier to comment on details in various ways, including GitHub's comment feature.
   (Just beware---Markdown interprets a line that ends with two spaces as a hard line break.)
1. Maruku automatically does "smartypants"-style filtering.
   That means "smart quotes" as in Word and Pages.
   Three dots are automatically converted to a true ellipsis character: ...
   Two dashes are converted into an en-dash: --
   Three dashes are converted into an em-dash: ---
1. If you want to include a quotation that is called out visually, use blockquote syntax.
   If you include an attribution for that quotation, mark it up this way:
   <pre>
&gt; Luck is the residue of design.
&gt; 
&gt; ---Branch Rickey
&gt; {: .attribution}
</pre>
   That assigns the "attribution" CSS class to the last paragraph of the blockquote.
   The styles we use will handle it appropriately.
1. Speaking of quotes: I've pulled most of the links to quoted books and resources into
   `_includes/references.md`, and included that at the bottom of the top-level pages.
   Not every reference needs to go there, but doing so allows us to quote the same resource
   in multiple places, with improved consistency and reduced chance of error.
   And it keeps the other files cleaner.
1. Maruku gives all headings an 'id' attribute.
   By default, the id is generated (apparently) by stripping all punctuation from the heading text,
   converting strings of whitespace to underscores, and lowercasing.
   (Or something like that.)
   If you need to link directly to a heading using a fragment identifier,
   the automatically generated id is often unsuitable.
   (And even if it's fine for now, changing the heading text later will break links.)
   So if you need to link directly to a heading within a larger document, assign an explicit id:
   <pre>## "Here's a nickel. Call someone who cares." {: #complaints}</pre>
1. As of 2009/07/22, the version of Maruku that they're using on GitHub doesn't deal correctly
   with reference-style links.
   If you have a space in your link label, Maruku gets confused.
   In order for it to work correctly, I had to add aliases in `references.md`
   for labels that contain spaces.
   (The aliases simply use underscores instead of spaces.)
   The original labels containing spaces are still necessary so that implicit link names work.