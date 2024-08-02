# Glitch

If you use the segment in MD mode with animations on an iOS device (or simulator), there is a bounce
style glitch when you select the first or last item in the list.

## Steps to Replicate

- clone this repo
- `npm i`
- `npm run build`
- `npx cap open ios` : build and run on a device or simulator

In the app:

- select "Member Benefits" - scrolling is smooth
- select "See What's New" - at this point you will see a bounce glitch
- select "Member Benefits" - scrolling is smooth
- select "Discounts" - scrolling is smooth
- select "Travel" or "Via" - at this point you will see a bounce glitch

If you want to see this working with smooth scrolling across the board, I have a branch using Ionic v6
and it works fine there.

- `git checkout ionic6`
- `npm i`
- `npm run build`
- `npx cap open ios` : build and run on a device or simulator

Repeat the above steps, but the scrolling you see should be smooth the whole time.
