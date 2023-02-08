This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

This repo replicates a TypeScript bug as described in [`this MUI ticket`](https://github.com/mui/material-ui/issues/36043#issuecomment-1420682564).

## To reproduce the bug:

1. Open /src/icons/AircraftPrivateJetMd-broken.tsx
2. Run `yarn install`
3. Run `yarn build` or `yarn next build` to make sure the build is successful
4. Uncomment the commented out code from line 3
5. Comment out lines 1 and 2 (the null component export)
6. Run `yarn build` or `yarn next build` again to see the build hang