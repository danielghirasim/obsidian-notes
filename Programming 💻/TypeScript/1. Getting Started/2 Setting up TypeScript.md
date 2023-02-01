Download project included in course

![[Pasted image 20230201185013.png | 700 ]]

If you use the app as it is, this will not produce the wanted result since this function is concatenating 2 strings. If you access the value of an input element in JS, it is <mark style="background: #ff79c6;">ALWAYS</mark> a string.

<mark class="hltr-coolorange">Steps to use TS: </mark>
- Install node.js
- Use npm to install TS globally on our machine using the command `npm i -g typescript`
- Add a new file with the `.ts` extension
- In the terminal write `tsc ts-only.ts` => this will create a .js file with the same name
- Link your new file in index.html

Note: To start watch mode just write `tsc filename.ts -w`

Notice in the picture below that by simply copying the code over to a .ts file, VSCode already highlights some possible problems our code might have

![[Pasted image 20230201195042.png | 700 ]]

<mark class="hltr-coolorange">A few things to note here :</mark>
- We added `!` telling TS that we are "sure we are getting an element" also meaning we will never get null (this is referring to the DOM input element)
- We use `as HTMLInputElement` also know as type casting letting TS know that this will be the type of `HTMLInputElement`
- The parameters of the function now have a `: number` telling the compiler that it will be a number

If we don't do the steps above then we will get a compilation error when using the TS command

This is how our compiled code looks like:

![[Pasted image 20230201195919.png | 700]]
