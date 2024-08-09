# RYZE Digital Scss Utilities

![Run linter(s) workflow status](https://github.com/ryze-digital/scss-utilities/actions/workflows/run-lint.yml/badge.svg)

## Install

```sh
npm i @ryze-digital/scss-utilities
```

## Usage

```scss
@use "@ryze-digital/scss-utilities";
```
Use provided configuration mixin to configure your global project defaults.

```scss
@include scss-utilities.configure(...);
```

See [/src/_config.scss](src/_config.scss) for all possible configuration options.

## Example

Let's say you want your blockquotes to always use the quotation marks associated with the current language.

```scss
blockquote {
    @include scss-utilities.quotes();
}
```