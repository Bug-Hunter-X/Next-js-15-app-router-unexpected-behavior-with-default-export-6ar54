# Next.js 15 App Router Unexpected Behavior

This repository demonstrates an unexpected behavior in Next.js 15's App Router when using a default export in the `pages` directory.  The issue occurs when navigating to the root path.  The default export is not rendered as expected.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `http://localhost:3000/`

The expected behavior is to see "Hello world" rendered on the page.  However, the actual behavior is a blank page or an error.

## Solution

The solution is to rename the pages/index.js file to app/page.js and use the new file structure from the Next.js 13+ app directory