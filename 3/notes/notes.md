**1**. What is JSX ?
   - It is HTML like syntax extension to javascript
   - behind the scenes, it gets converted to React.createElement() calls via Babel compiler
   -It produces React elements
   - JSX is not necessary in React. It is just syntactic sugar for React.createElement
   - We can put any JS expression inside {} curly braces of JSX
   - JSX is itself an expression, which becomes regular JS function call and evaluate to JS objects.
   - Thus we can use JSX inside if statements, loops, assign to variable, accept it as arguments and return JSX from functions.

**2**. Superpowers of JSX
   - It makes code easy to read, maintain
   - HTML like syntax, easier to write, debug.
   - It accepts properties like attributes in HTML, thus easier to pass data from parent to child.
   - evaluates to JS expression at the end, thus acts like a value to variable, flexibility.

**3**. Role of type attribute in script tag ? What options does it have ?   
   - script tag is used to embed executable code or data, typically used to embed or refer to JS code.
   - 'type' indicates the type of script represented: a classic script, a JavaScript module, an import map, or a data block
   - we have default as MIME type, which is to be omitted if script refers to JS code.
   - type - module: causes the code to be treated as JS module. There is no need to use the defer attribute,when loading a module script; modules are deferred automatically.
   - third type is importmap: indicates body of the element contains an import map. Usually for developers to control resolving of module imports by the browser.

**4**. `<TitleComponent> vs <TitleComponent/> vs <TitleComponent> </TitleComponent>`
   - First one is invalid syntax, since we require JSX to have closing character '/'
   - Second one is valid JSX
   - Third one is also valid, we use such syntax, when React Component is parent component, and we need to include some child elements or components in it.