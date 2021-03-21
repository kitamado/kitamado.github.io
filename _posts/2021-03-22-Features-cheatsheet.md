---
title: Features cheatsheet
tags: memo
---
### Custom Features
1. **wiki-style link**
   - Internal links: `[​[​Some Link]]`
   - External links: `[​[​Some Text::https://address-to-the-website]]`
  
2. **sidenote & marginnote**
   Keywords: `lsn`,`rsn`,`lmn`,`rmn`
   - Sidenote: `[​[Some Text::keyword-of-the-type-of-the-sidenote]]`
   - Marginnote: `[​[​Some Text::keyword-of-the-type-of-the-marginnote]]`
  
3. **highlight**
   - `[​[​Some Link::highlight]]`
  
4. **partial Transclusion**
   - Sidenote-transclusion: `[​[Some Text::keyword-of-the-type-of-the-sidenote-transclusion]]`
   - Marginnote-transclusion: `[​[​Some Text::keyword-of-the-type-of-the-marginnote-transclusion]]`
  
5. **warp**
   - `[​[Some Text::wrap]]`
  
6. **flash card**
   - **[​[**Some Text**::srs]]**
  
7. **specific classes** for changing font-type, font-size, and font-weight
   ```
   {:.large}
    Some text here that needs to be enlarged
   ```
   - size include: [[very-small, medium-small, small, small-medium, medium, medium-large, large, very-large::highlight]]
   - font include: [[regular-sans, serif, bold, italic, oblique, bolder, etc. ::highlight]]
   - other: [[.boxit, .disable-user-select , etc.::highlight]]
  
8. **Auto-tagging WIP posts on the feed**
   - add `status: ongoing` in YAML front.

### Auto Features
1. **Related Posts**: Posts that share same tag(s).
2. **Linked References(Backlinks)**: Posts that link other posts inside your blog.
3. **On-feed context menu**
4. **On-hover page preview**
5. **Omnisearch bar**

### Markdown
1. Underscore
    Markdown doesn't have raw underscore syntax, use inline HTML instead:
   - Raw Text: `<u>Underlined Text</u>`
   - Rendered Text: <u>Underlined Text</u>;