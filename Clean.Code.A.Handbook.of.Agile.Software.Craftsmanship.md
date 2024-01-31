
## 1. Clean code

**Bad code**

We know what bad code is. And we all know the impact of bad code. 

**Definition of clean code**
- Elegant end efficient
- Can be read and enhanced by other devs
- No duplication, one thing, expressiveness, tiny abstraction.
- ...

>. . . pretty much what you expected.

Indeed, it is what you expected it to be when read.

**Practice**

>Try and leave this world a little better than you found it . . .

Actively cleaning code. If we keep our code clean, we dont need a big cleanup.

## 2. Meaningful Names

Things should be named with an intent

**Avoid Disinformation**

Avoid words which meaning may varies, avoid names that vary in small ways.

Do have consistency in spellings.

**Make Meaningful Distinctions**

Avoid meaningless name (*a*, *a1*, etc.)

Avoid noise word: if there is already a `Product`, then `ProductInfo` or `ProductData` doesn't mean anything different!

Avoid having data types in name (unless maybe for weakly typed languages, like JS?)

**Use Pronouceable Names**

As title

**Use Searchable Names**

The length of a name should correspond to the size of its scope. If a variable is used in multiple places, then it is better to give it a search-friendly name (meaning less likely there is anything named similar in difference context).

**Avoid Encoding**

If we take time to encode things, we have to carry extra burden of deciphering it.

Example: `UserRepositoryImpl`, while it is fine, if one implementation is likely, use `DefaultUserRepository` instead because it have a meaning.

**Avoid Mental Mapping**

As title, don't invent old things.

**Class Name**

Should be a noun. Should not have ambiguous word like `Manager`, `Data`, etc.

**Method Names:** should be a verb

**Dont be cute:** don't be too clever

**Pick One Word per Concept:** as title

**Don't Pun:** avoid using same word for two purpose

**Use Solution Domain Names:** stick to "programmer" terms

**Use Problem Domain Names:** if there is none, use "bussiness" terms

**Add meaningful Context:** if the name is not clear enough, you can add some context to it 

**Dont Add Gratuitous Context:** dont overdo the previous point!

## 3. Function
Function should show it *intent*, and readable by human, of course.

**Small:** Function should be small, you know that

**Blocks and Indenting:** If your code is nested, maybe you should split it to functions. More readable, and each block have nice descriptive name.

**Do one thing:** if we can extract another function from it with a name that is not a restatement of it implementation