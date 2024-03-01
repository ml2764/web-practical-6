# Practical 6 (Week 3) - Grid & Design

In this practical you will gain hands on experience with the CSS grid module in combination with flexbox and media queries.

## Stage 1: Grid Familiarisation 
Open [Grid Garden](https://cssgridgarden.com/). Try to complete all 28 levels.

## Stage 2: Creating a Responsive Layout Using, Grid, Flexbox, and Media Queries
Make a new copy of the York University Press website you created in last week's practical. It is OK if you didn’t quite finish the last practical yet; start with what you have. 

### Exercise 2.1: Make the grid
Consider how you could modify the CSS to use a grid to layout the overall page. You will still need flexbox in a few places. Here are some suggestions:
- Make `#content-area` the grid container by setting its `display` property to grid.
- The grid should have two columns, 75% and 25% wide respectively. If you put `<main>` and `<aside>` into a container div to help with layout in a previous practical, remove that div now.
- `<header>`, `<nav>`, and `<footer>` should all span both columns.

Your page should look pretty much the same as before on a large device.

### Exercise 2.2: Make the grid responsive
Run the website in Chrome using the Live Preview extension and open the device simulator, which you can find in Developer Tools. Set the device simulator to responsive mode then view the site at different breakpoints by clicking the grey bars above the site. 

Most of the media queries you added last time should still work with the new grid-based content area. However, you will notice one key issue if you compare the new layout to the responsive layouts created last practical. Previously, the `<aside>` dropped below `<main>` on medium-sized devices (tablet – 768px) and below. Now, both columns appear side by side. Your task is to fix this issue using media queries. 
Tips:
- If you look at the screenshots of my responsive layouts from last practical, you will notice that the responsive layout is essentially a single column.
- You may be tempted to reduce the grid size from two columns to one by changing the `grid-template-columns` property for devices less than 768px wide. Although this is valid, you will find this change has knock on effects that also need to be fixed. There is a simpler solution that only involves changing a single property on a single element…
- An alternative approach is to consider using the grid layout only on devices larger than 768px as a single column grid is essentially not a grid. This approach will result in the cleanest CSS. If you go this route, you will need media queries that use the `min-width` property of the device.

## Stage 3: Update Your Portfolio Layout
Open up the portfolio site that you last worked on in previous practicals. Use either or both layout approaches we have covered this week to create the layout of your site. Be sure to check how your portfolio looks on small devices and use media queries to make your site responsive. 

You may also wish to consider how your portfolio design makes use of the visual design principles we talked about in class this week, especially your use of negative space, fonts, and colours.
