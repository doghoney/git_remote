# __MARKDOWN grammer__
### author : shin jun ho
### student number : 20202908

## __heading__
>1\. add number signs (#) in front of a word or phrase.  
>2. The number of number signs you use should correspond to the heading level.  
>3. put space between # and a word or phrase.  

- example  

        # Heading level 1  
        ## Heading level 2  
        ### Heading level 3  

- ### alternate syntax

    >1\. add any number of == characters for heading level 1.    
    >2. add any number of -- characters for heading level 2.  

    - example  

            Heading level1  
            ==  
            Heading level2  
            ---  

## __paragraphs__  
>1\. use a blank line to separate one or more lines of text.    
>2. don’t indent paragraphs with spaces or tabs.  
- do   

        I really like using Markdown.  

        I think I'll use it to format all of my documents from now on.  
- do not   

            This can result in unexpected formatting problems.  

      Don't add tabs or spaces in front of paragraphs.  

## __linebreak__  
>two options    
>\- use two or more spaces after line.   
>\- use \<br> after line.   
- example   

        First line with two spaces after.__  
        And the next line.  

        First line with two spaces after.<br>  
        And the next line.  

## __emphasis__  
- **bold**  
    >1\. add two asterisks or underscores before and after a word or
    phrase.   
    >2. without spaces around the letters.   
    - ex  

            I just love **bold text**.  
            I just love __bold text__.  

- *italic*  
    >1\. add one asterisk or underscore before and after a word or phrase.  
    >2. without spaces around the letters.  
    - ex   

            Italicized text is the *cat's meow*.  
            Italicized text is the _cat's meow_.  

- ***bold & italiic***  
    >1\. add three asterisk or underscore before and after a word or phrase.  
    >2. without spaces around the letters.  
    - ex  

            This text is ***really important***.  
            This text is ___really important___.  
            This text is __*really important*__.
            This text is **_really important_**.  

## __blockquotes__
>add a > in front of a paragraph.  
- example  

        > Dorothy followed her through many of the beautiful rooms in her castle.  

    > Dorothy followed her through many of the beautiful rooms in her castle.  

- ### multiple paragraphs  
    > add a > on the blank lines between the paragraphs.
    - example

            > Dorothy followed her through many of the beautiful rooms in her castle.
            >
            > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

        > Dorothy followed her through many of the beautiful rooms in her castle.
        >
        > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

- ### nexted blockquotes
    > add a >> in front of the paragraph you want to nest.
    - example

            > Dorothy followed her through many of the beautiful rooms in her castle.
            >
            >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
        > Dorothy followed her through many of the beautiful rooms in her castle.
        >
        >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

- ### blockquotes with otehr elements
    >\<warning> Not all elements can be used.   
    >it needs to be experimented to see which ones work.

        > #### The quarterly results look great!
        >
        > - Revenue was off the chart.
        > - Profits were higher than ever.
        >
        >  *Everything* is going according to **plan**.
    > #### The quarterly results look great!
    >
    > - Revenue was off the chart.
    > - Profits were higher than ever.
    >
    >  *Everything* is going according to **plan**.

## __list__
- ### ordered
    >1\. add line items with numbers followed by periods.  
    >2. The numbers don’t have to be in numerical order.  
    >3. the list should start with the number one.  

    - ex

            1. First item
            8. Second item
            3. Third item
            5. Fourth item
    - rendered output :   
        1. First item
        8. Second item
        3. Third item
        5. Fourth item

- ### unordered
    >1\. add dashes (-), asterisks (*), or plus signs (+) in front of line items.  
    >2. indent one or more items to create a nested list.  
    >3. don’t mix and match delimiters in the same list

    - ex

            - First item
            - Second item
            - Third item
                - Indented item
                - Indented item
            - Fourth item
    - rendered output :
        - First item
        - Second item
        - Third item
            - Indented item
            - Indented item
        - Fourth item

- ### adding elements
    > indent the element four spaces or one tab
    - paragraphs  

            *   This is the first list item.
            *   Here's the second list item.

                I need to add another paragraph below the second list item.

            *   And here's the third list item.

    - blockquotes

            *   This is the first list item.
            *   Here's the second list item.

                > A blockquote would look great below the second list item.

            *   And here's the third list item.

    - code blocks

            1.  Open the file.
            2.  Find the following code block on line 21:

                    <html>
                      <head>
                        <title>Test</title>
                      </head>

            3.  Update the title to match the name of your website.

    - images

            1.  Open the file containing the Linux mascot.
            2.  Marvel at its beauty.

                ![Tux, the Linux mascot](/assets/images/tux.png)

            3.  Close the file.

    - lists

            1. First item
            2. Second item
            3. Third item
                - Indented item
                - Indented item
            4. Fourth item

## __`code`__
>enclose it in backticks (`)  
- example

        At the command prompt, type `nano`.

- ### escaping backticks
    >If the word or phrase you want to denote as code includes one or more backticks,  
    >you can escape it by enclosing the word or phrase in double backticks (``).

    - ex

            ``Use `code` in your Markdown file.``

    - rendered output :   
        ``Use `code` in your Markdown file.``

- ### codeblocks
    >indent every line of the block by at least four spaces or one tab.

    - ex

            ____<html>
            ____  <head>
            ____  </head>
            ____</html>
    - renederd output :  

            <html>
              <head>
              </head>
            </html>

## __horizontal rules__
>1\. use three or more asterisks, dashes, or underscores on a line by themselves.  
>2. put blank lines before and after horizontal rules.

- example

        ***

        ---

        _________________

- rendered output :
    ***

    ---

    _________________

## __links__
>1\. enclose the link text in brackets (e.g., [Naver])  
>2. follow it immediately with the URL in parentheses (e.g., (https://naver.com)).)

- ex

        My favorite search engine is [Naver](https://naver.com).

    My favorite search engine is [Naver](https://naver.com).

- ### adding titles
    >1\. enclose it in parentheses after the URL.  
    - ex

            My favorite search engine is [Naver](https://naver.com "The best search engine for korean").  
    - rendered output :
        My favorite search engine is [Naver](https://naver.com "The best search engine for korean").

- ### urls and email addresses
    >To quickly turn a URL or email address into a link,
    >enclose it in angle brackets.
    - ex

            <https://www.markdownguide.org>
            <fake@example.com>
    - rendered output :  
        <https://www.markdownguide.org>  
        <fake@example.com>

- ### formatting links
    >emphasize links:  
    >- add asterisks before and after the brackets and parentheses.  
    >
    >denote links :
    >- add backticks in the brackets.

    - ex

            I love supporting the **[EFF](https://eff.org)**.
            This is the *[Markdown Guide](https://www.markdownguide.org)*.
            See the section on [`code`](#code).
    - rendered output :  
        I love supporting the **[EFF](https://eff.org)**.  
        This is the *[Markdown Guide](https://www.markdownguide.org)*.  
        See the section on [`code`](#code).  

- ### reference-style links
    - first part

            [hobbit-hole][1]
            [hobbit-hole] [1]
    - second part
        >1. The label, in brackets, followed immediately by a colon and at least one space (e.g., [label]: ).
        >2. The URL for the link, which you can optionally enclose in angle brackets.
        >3. The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

            [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
            [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit             lifestyles"
            [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit             lifestyles'
            [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit             lifestyles)
            [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle>           "Hobbit lifestyles"
            [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle>           'Hobbit lifestyles'
            [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle>           (Hobbit lifestyles)

    - example of plutting together  
        - standard  

                In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
                of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
                eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.  

        - fixed :  

                In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
                of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
                eat: it was a [hobbit-hole][1], and that means comfort.

                [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"  
    - ### cf)  
        >try to URL encode any spaces with %20.  

        - do  

                [link](https://www.example.com/my%20great%20page)  
        - do not  

                [link](https://www.example.com/my great page)  

## __images__
>1\. add an exclamation mark (!)   
>2. followed by alt text in brackets, [ ]    
>3. and the path or URL to the image asset in parentheses. ( )  
>\+ optionally add a title after the URL in the parentheses.  
- example    

        ![I am cat!](./cat.jpg "Cute Cat")   
- rendered output :   
![I am cat!](./cat.jpg "Cute Cat")  

## __linking images__
> enclose the Markdown for the image in brackets, and then add the link in parentheses.

- example

        [![I am cat!](./cat.jpg "Cute Cat")](https://pixabay.com/photos/cat-young-animal-curious-wildcat-2083492/)

- rendered output :
[![I am cat!](./cat.jpg "Cute Cat")](https://pixabay.com/photos/cat-young-animal-curious-wildcat-2083492/)       

## __escaping characters__
>To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (\) in front of the character.

- characters you can escape  
    - \\	  
    - \`
    - \*	  
    - \_
    - \{ }
    - \[ ]	  
    - \< >
    - \( )
    - \#
    - \+
    - \-
    - \.
    - \!
    - \|

## __HTML__
>Many Markdown applications allow you to use HTML tags in Markdown-formatted text.

- example

        This **word** is bold. This <em>word</em> is italic.
- rendedr output :  
    This **word** is bold. This <em>word</em> is italic.

[GitHub repository URL](https://github.com/doghoney/softwareengineering/blob/main/README.md "go to Github")
