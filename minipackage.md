# minipackage

A minipackage is an npm package as follows:

1. The package contains just one source file, `index.js`. `index.js`
   exports a single function or JSON-serializable data structure.

2. The package contains just one documentation file, a README. The
   README is in CommonMark format.

3. The package's tests are written literate-style, in fenced code blocks
   within `README.md`. The tests use Node.js' built-in `assert` module.
   An `npm `README.md`.test` script extracts and run the tests.

4. All tests are end-to-end. If it is worth testing separately, it
   belongs in a separate minipackage.

5. The package repository contains dotfiles, if any, only for
   configuring continuous integration and other testing services. Those
   files are excluded from the published package using a `files` array
   in `package.json`.
