# Issue Reproduction

```bash
$ npm i
$ npm run build
$ npm run start
# Open http://localhost:3000/
# Find open document.querySelector('meta[property="og:image"]').getAttribute("content"): it displays a dog
$ cp opengraph-image.new.jpg app/opengraph-image.jpg
$ npm run build
$ npm run start
# Open http://localhost:3000/
# Find open document.querySelector('meta[property="og:image"]').getAttribute("content"): it displays a dog still instead of a cat
# The query string changed so there is an attempt to bust the cache.
$ rm -rf .next
$ npm run build
$ npm run start
# Open http://localhost:3000/
# Find open document.querySelector('meta[property="og:image"]').getAttribute("content"): it displays a cat as expected
```
