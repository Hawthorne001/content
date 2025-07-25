---
title: Doctype
slug: Glossary/Doctype
page-type: glossary-definition
sidebar: glossarysidebar
---

In {{Glossary("HTML")}}, the **doctype** is the required `<!doctype html>` preamble found at the top of all documents. Its sole purpose is to prevent a {{Glossary("browser")}} from switching into so-called ["quirks mode"](/en-US/docs/Web/HTML/Guides/Quirks_mode_and_standards_mode) when rendering a document; that is, the `<!doctype html>` doctype ensures that the browser makes a best-effort attempt at following the relevant specifications, rather than using a different rendering mode that is incompatible with some specifications.

The doctype is case-insensitive. The convention of MDN code examples is to use lowercase, but it's also common to write it as `<!DOCTYPE html>`.

## See also

- [Definition of the DOCTYPE in the HTML specification](https://html.spec.whatwg.org/multipage/syntax.html#the-doctype)
- [Quirks Mode and Standards Mode](/en-US/docs/Web/HTML/Guides/Quirks_mode_and_standards_mode)
- [Document.doctype](/en-US/docs/Web/API/Document/doctype), a JavaScript method that returns the doctype
