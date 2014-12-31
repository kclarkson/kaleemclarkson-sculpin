---
title: Dates in Sculpin 
tags: 
    - Sculpin 
    - Markdown
categories:
    - Front End
---
While retraining the brain to go old school with markdown and raw HTML. One thing I was looking for was the date posting. Come to find out Sculpin can read the URL of your post if written in a certain syntaxt.  In combination with the naming you can now use twig <code>date</code> filter you can unlock a ton of goodness. 

    namespace Foo;

    /**
     * Awesome Contrived Example.
     */
    class Bar implements BarInterface
    {
        private $baz;

        public function __construct(BazInterface $baz)
        {
            $this->baz = $baz;
        }

        public function doIt()
        {
            return $this->baz->do('it');
        }
    }

You can also use [fenced code blocks][fcb] with a syntax declaration at the top.
The markers are `~` instead of <code>`</code>.

[fcb]: http://michelf.ca/projects/php-markdown/extra/#fenced-code-blocks

~~~php
if ($fencedCodeBlock->syntax !== 'PHP') {
    throw new UnexpectedValueException("wat");
}
~~~
Like this addition to the skeleton? You can thank for [@Pawka](https://github.com/Pawka)
for suggesting it. :)
