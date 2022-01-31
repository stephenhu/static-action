# static action

github action for static.  static takes amber and markdown files and converts them into a single page html file complete with index page, navigation, page view, and other features.

this action can be incorporated into a number of workflows to automatically generate static content.

## inputs

### source

directory where source files exist, default uses the current directory

## outputs

## example usage

taken from 'github.com/stephenhu/blog-www' in directory '.github/workflows/build.yml'

```
jobs:
  build:
    runs-on: ubuntu-latest
  steps:
    uses: actions/checkout@v2 # this repository should contain your amber and markdown files
    uses: stephenhu/static-action@v1 # this step builds index.html out of these files.
```
  