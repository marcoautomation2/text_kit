# Text Kit

A library of small text helpers written in Fearless.
The demo is listed in the storefront https://marcoservetto.github.io/fearless_demos/ with the rank `core200`.

## Use

The URL of the zip is https://marcoautomation2.github.io/text_kit/text_kit_lib.zip.
The page https://marcoautomation2.github.io/text_kit/ has a button that copies the URL.
Import the URL into a Fearless project with the Fearless manager.
The zip also works by hand: copy the zip, zipped or unzipped, into the project.
Write `use text_kit.Pads as Pads;` in the rank file of the package that needs `Pads`.
The package that uses the library needs a rank higher than `core200`.
Every package of rank `app` qualifies.

## The library

The package is `text_kit`.
- `Pads`: `.left`, `.right` and `.center` make a text as wide as asked.
- `Words`: `.of` splits a text into words, `.count` counts the words and `.title` capitalizes each word.
- `Slugs`: `.of` joins the lower case words of a text with dashes.
- `Truncs`: `.to` shortens a text that is too long.

Every method has examples in its doc comment.
Running the folder `project` checks the examples.
A package inside a zip gets no generated checks, so check the examples with the unzipped folder `project`.

## The example

The folder `example` is a small app that uses the library.
Copy `text_kit_lib.zip` into the folder `example`, or copy the folder `project/_text_kit` into the folder `example`.
Run the folder `example`.

## Deployment

Each push to `main` runs `.github/workflows/pages.yml`.
The workflow zips the folder `project` into `text_kit_lib.zip`.
The workflow publishes the zip and `site/index.html` on GitHub Pages.
