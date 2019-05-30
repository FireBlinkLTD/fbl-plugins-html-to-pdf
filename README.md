# FBL Plugins: HTML to PDF

Allows to convert any HTML document into PDF file inside [fbl](https://fbl.fireblink.com) flow.

[![CircleCI](https://circleci.com/gh/FireBlinkLTD/fbl-plugins-html-to-pdf.svg?style=svg)](https://circleci.com/gh/FireBlinkLTD/fbl-plugins-html-to-pdf) [![Greenkeeper badge](https://badges.greenkeeper.io/FireBlinkLTD/fbl-plugins-html-to-pdf.svg)](https://greenkeeper.io/)
[![codecov](https://codecov.io/gh/FireBlinkLTD/fbl-plugins-html-to-pdf/branch/master/graph/badge.svg)](https://codecov.io/gh/FireBlinkLTD/fbl-plugins-html-to-pdf)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/FireBlinkLTD/fbl-plugins-html-to-pdf.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/FireBlinkLTD/fbl-plugins-html-to-pdf/alerts/)
[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/FireBlinkLTD/fbl-plugins-html-to-pdf.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/FireBlinkLTD/fbl-plugins-html-to-pdf/context:javascript)

## Integration

There are multiple ways how plugin can be integrated into your flow.

### package.json

This is the most recommended way. Create `package.json` next to your flow file with following content:

```json
{
  "name": "flow-name",
  "version": "1.0.0",
  "description": "",
  "scripts": {
    "fbl": "fbl"
  },
  "license": "UNLICENSED",
  "dependencies": {
    "@fbl-plugins/html-to-pdf": "1.0.0",
    "fbl": "1.7.0"
  }
}
```

Then you can install dependencies as any other node module `yarn install` depending on the package manager of your choice.

After that you can use `yarn fbl <args>` to execute your flow or even register a custom script inside "scripts".

### Global installation

`npm i -g @fbl-plugins/html-to-pdf`

### Register plugin to be accessible by fbl

- via cli: `fbl -p @fbl-plugins/html-to-pdf <args>`
- via flow:

```yaml
requires:
  fbl: '>=1.7.0'
  plugins:
    '@fbl-plugins/html-to-pdf': '>=1.0.0'

pipeline:
  # your flow goes here
```

## Documentation

Read more [here](docs/README.md).
