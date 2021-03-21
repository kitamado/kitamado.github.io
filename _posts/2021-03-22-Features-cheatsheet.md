---
title: Features cheatsheet
tags: Memo
---
### Custom Features
1. wiki-style link
   - Internal links: **[​[**​Some Link**]]**
   - External links: **[​[**​Some Text::https://address-to-the-website**]]**
2. sidenote & marginnote
   - Sidenote: **[​[**Some Text**::keyword-of-the-type-of-the-sidenote]]**
   - Marginnote: **[​[**​Some Text::**keyword-of-the-type-of-the-marginnote]]**
3. highlight
   - **[​[**​Some Link**::highlight]]**
4. partial Transclusion
   - Sidenote-transclusion: **[​[**Some Text**::keyword-of-the-type-of-the-sidenote-transclusion]]**
   - Marginnote-transclusion: **[​[​**Some Text**::keyword-of-the-type-of-the-marginnote-transclusion]]**
5. warp
   - **[​[**Some Text**::wrap]]**
6. flash card
   - **[[**Some Text**::srs]]**
7. specific classes for changing font-type, font-size, and font-weight
   ```
   {:.large}
    Some text here that needs to be enlarged
   ```
   size include: [[very-small, medium-small, small, small-medium, medium, medium-large, large, very-large::hightlight]]
   font classes include: [[regular-sans, serif, bold, italic, oblique, bolder, etc. ::highlight]]
   other: [[.boxit, .disable-user-select , etc.::highlight]]



### Markdown
#### Underscore
Markdown无下划线原生语法， 因为会和链接的默认样式产生混淆。
解决方法是使用行内HTML:
- Raw Text
    ```
    <u>Underlined Text</u>
    ```
- Rendered Text
  <u>Underlined Text</u>;