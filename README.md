# Web components SEO
### Testing indexability of web components.

This website tests how standard and custom HTML tags are indexed by Google under different circumstances.


## Standard HTML

| Content          | Javascript | Link                                                                                    | Seen by Google |
|------------------|------------|-----------------------------------------------------------------------------------------|----------------|
| async javascript | ES5        | [/html-dynamic-async](https://leofavre.github.io/web-components-seo/html-dynamic-async) | no             |


## Custom HTML

| Content          | Tag definition | Shadow DOM | Javascript | Link                                                                                                    | Seen by Google |
|------------------|----------------|------------|------------|---------------------------------------------------------------------------------------------------------|----------------|
| sync javascript  | immediate      | no         | ES5        | [/noshadow-dynamic-sync-es5](https://leofavre.github.io/web-components-seo/noshadow-dynamic-sync-es5)   | no             |
| sync javascript  | immediate      | no         | ES6        | [/noshadow-dynamic-sync](https://leofavre.github.io/web-components-seo/noshadow-dynamic-sync)           | no             |
| sync javascript  | immediate      | yes        | ES5        | [/shadow-dynamic-sync-es5](https://leofavre.github.io/web-components-seo/shadow-dynamic-sync-es5)       | no             |
| sync javascript  | immediate      | yes        | ES6        | [/shadow-dynamic-sync](https://leofavre.github.io/web-components-seo/shadow-dynamic-sync)               | no             |
| async javascript | lazy           | no         | ES6        | [/noshadow-dynamic-async](https://leofavre.github.io/web-components-seo/noshadow-dynamic-async)         | no             |
| async javascript | lazy           | yes        | ES6        | [/shadow-dynamic-async](https://leofavre.github.io/web-components-seo/shadow-dynamic-async)             | no             |

### Conclusion

Google can always see static HTML content on the page, in standard or custom HTML tags.

When it comes to Javascript-rendered content, Google completely ignores custom HTML tags but not standard ones.