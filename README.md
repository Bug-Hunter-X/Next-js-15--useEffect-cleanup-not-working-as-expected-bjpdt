# Next.js 15 useEffect Cleanup Issue

This repository demonstrates a bug encountered in a Next.js 15 application where a `useEffect` hook's cleanup function doesn't seem to work correctly when navigating away from and back to a page.  The counter on the About page continues to increment even after leaving the page and returning.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to the About page.
5. Navigate to the Home page.
6. Navigate back to the About page.  Observe that the counter continues to increment from where it left off instead of restarting.

## Expected Behavior

The counter should restart when navigating back to the About page.  The `useEffect` cleanup function should properly clear the interval timer when the component unmounts.

## Potential Solutions (and why they may not work)

While the provided `useEffect` cleanup function appears correct, there's a possibility of issues relating to component lifecycle or the way Next.js handles routing in version 15. Further investigation is needed.  The solution file may contain a resolution. 