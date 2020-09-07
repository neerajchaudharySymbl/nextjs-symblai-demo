## Notes

The CSS classes generated by Emotion will include the tailwind styles but not the name of the classes. For example the following component:

```jsx
const Header = styled.div`
  ${tw`font-mono text-sm text-gray-800`}
`
```

Will be transformed into:

```css
.css-25og8s-Header {
  font-family: Menlo, Monaco, Consolas, 'Liberation Mono', 'Courier New',
    monospace;
  font-size: 0.875rem;
  color: #2d3748;
}
```

### tailwind CSS config

Use the following command when you add a tailwind plugin that adds to tailwind's base css:

```bash
npm run build:base-css
# or
yarn run build:base-css
```
