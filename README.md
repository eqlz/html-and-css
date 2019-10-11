# CSS
## Position

### Position
| Position | Removed from flow of document | Relative to |
| --- | --- | --- |
| relative | No, treated as still in normal flow | Relative to the element's original position
| absolute | Yes, treated by other elements as it was not there | Relative to the nearest positioned ancestor, ie, nearest non-static ancestor. If such ancestor can't be found, the element will be relative to document
| fixed | Yes, treated by other elements as it was not there | Relative to the document. The element will not be affected by scrolling. 

### Example

absolute
<p class="codepen" data-height="265" data-theme-id="0" data-default-tab="js,result" data-user="eqlzh" data-slug-hash="LYYVZNK" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="css-position-absolute">
  <span>See the Pen <a href="https://codepen.io/eqlzh/pen/LYYVZNK">
  css-position-absolute</a> by Emily (<a href="https://codepen.io/eqlzh">@eqlzh</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>

fixed
<p class="codepen" data-height="265" data-theme-id="0" data-default-tab="html,result" data-user="eqlzh" data-slug-hash="NWWqRdE" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="css-position-fixed">
  <span>See the Pen <a href="https://codepen.io/eqlzh/pen/NWWqRdE">
  css-position-fixed</a> by Emily (<a href="https://codepen.io/eqlzh">@eqlzh</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>

## Selector
* Descendant combinator
* Child combinator
* pseudo class
* pseudo element

### Example
<p class="codepen" data-height="265" data-theme-id="0" data-default-tab="css,result" data-user="eqlzh" data-slug-hash="OJJVRjo" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="css-selectors">
  <span>See the Pen <a href="https://codepen.io/eqlzh/pen/OJJVRjo">
  css-selectors</a> by Emily (<a href="https://codepen.io/eqlzh">@eqlzh</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>

## box-sizing
|  | Explanation | Dimension of the element | Example |
| --- | --- | --- | --- |
| content-box | Width, height properties include content, not including padding, border, margin | Width = width of the content Height = height of the content | .box {width: 350px; border: 10px solid black;} renders a box that is 370px wide.|
| border-box | Width, height properties include content, padding, border, not including margin|width = width of the content + padding + border Height = height of the content + padding + border| .box {width: 350px; border: 10px solid black;} Render box 350px wide, the width of content is 330px = 350 - (2 * 10px) |