# ki365.github.io

Official website for Ki365: The Engineering Collaboration Platform

## Structure

```
- docs: documentation pages
- website: main website pages
```

## Documentation Site

This website is built with [Hugo](https://gohugo.io/) as the SSG framework and [Hextra](https://imfing.github.io/hextra/) as the documentation theme.

## Development

To run the hugo development server run:

```
hugo server -s ./docs --buildDrafts --disableFastRender
```

To add a new page run:

```
hugo new content/docs/{new_content_filename}.md
```
