---
lang: en
title: Building a prototype in Figma
viewport: width=device-width, initial-scale=1.0
---

# As a class, build a Figma prototype for Planet Diner

## Tips

- be sure to name components
- be sure to name layers
- be sure to name frames
- To duplicate an art board, [alt]{.kbd} + click + drag on Windows,
  [option]{.kbd} + click + drag on Mac
- check the properties pane to make sure things are positioned and
  appear as they should

Before you start, look at what you have to do and plan how you will proceed.
Study the mock-up. What do you need to do here? Look for anything that is used more than once. These are candidates for reusable components or styles.

## Pages

### Cover page

This is what gets displayed when you look in your Figma projects. It's a good place for a thumbnail of your project.

### Content page

Typically, I would not have a content page. It is here to save student's time. You can drag what you need into you prototypes without having to import text and images.

### Assets page

These are images and illustrations I have imported into the project. I usually turn these into components. That way, if I need to swap something out, it will update everywhere.

### Design system page

These are base elements that get applied to components. Typically, it's colours and typography. Technically components are also part of the design system. I prefer to keep these base elements separate.

### Components

These are the elements that get reuses throughout the project. As a general rule of thumb, if you see something used more than once, make a component out of it.

### Mobile

This is where I build the prototype. I do one prototype per page. So a desktop version would be on its own page.

## Getting started

There is a menu on every page, including home. I note from the mockup that the menu has an open state and a closed state. When I look at the components page, I see that there are components for the header and menu states, but this can be taken further by having components that combine the header and the menu. The first thing I do is make two new components.

## Header with menu components

1. go to components page
2. open the assets pane so you can see components
3. drag an instance of the header onto the screen
4. drag an instance of the hamburger menu icon and place it on the image, properly aligned
5. drag another instance of the header onto the screen
6. drag an instance of the menu open and place it over the header image from step 5
7. Align the header image from step 3 and step 5, this will make it easier to align the menu
8. under the Figma menu, go to view and select _Rulers_
9. Place your cursor on the ruler at the top and drag a guide down to where you want the menu icons on the header image
10. align both menus vertically to the guide
11. center each menu with the header image it's on
12. select the image and closed menu, make a component called `header/nav-closed`
13. select the image and open menu, make a component called `header/nav-open`

> In a future class, we will learn how to make component sets. Component sets extend the power of components in Figma

## Build the home page with the navigation closed

1. delete the header image on the frame
2. delete the hamburger menu on the frame
3. from the asset panel, drag an instance of `header/nav-closed` and place it in the frame
4. in the layers panel, drag the header image so it is under the intro text
5. rename the home frame to _Header/nav-open_
6. make a copy of frame _Header/nav-open_ and call it _Header/nav-closed_

## Build the home page with the navigation open

1. on _Header/nav-closed_ replace the header with the _Header/nav-open_ component
2. fix the layer order
3. move the intro text and footer down so they leave space below the navigation menu
4. select the entire _Header/nav-open_ and resize it so the footer is completely within the frame

## Build the pizza menu closed page

1. Add a new frame, use iPhone 13 & 14, 390 x 844
2. Name the frame _pizza/menu closed_
3. With the frame still selected, select the colour _page/background_ (hover over the fill section on the properties panel, a grid icon will appear. Click this to ses the colours available in the library)
4. Drag components for _Header/nav-closed_, _menu items > Pizza_ and _Footer_ onto the artboard, position and align
5. resize the frame so the footer is in frame

## Build the pizza menu open page

1. Follow the same steps you did for _Pizza menu closed_ but use the _Header/nav-open_ component
2. name the frame _Pizza/menu-closed_

## Build Burgers menu open and burgers menu closed frames

Follow the same steps you took for _Pizza/menu-open_ and _Pizza/menu-closed_. Use the _Menu item > burgers component_ and use the same naming pattern for the frame names.

## Build Dessert menu open and dessert menu closed frames

Follow the same steps you took for _Pizza/menu-open_ and _Pizza/menu-closed_. Use the _Menu item > desserts component_ and use the same naming pattern for the frame names.

> **TIME SAVING TIP**
>
> For building Burgers and desserts frames a faster way to work is:
>
> 1. duplicate the frames you made for pizza
> 2. name the frames using the naming convention
> 3. on one of the new frames you create, select the pizza component and right click. From the context menu, choose _Swap instance_ and choose burgers or dessert

## Building the prototype

Before you begin, think about how the prototype frames will be linked. Think about what should happen for every interaction a person will have with the site. For example, if I'm on the home page, and I open the menu, but don't want to select any of the food options, how do I close the menu again? Remember, every interaction should have a way to return to the previous state.

Switch to prototype mode (it's a tab at the top of the properties panel beside _Design_)

For each connection in the prototype, choose the following settings

1. on tap
2. navigate to
3. _select the page you want to navigate to_
4. smart animate
5. ease out

You will need a connection for each of the following:

### Home/ nav closed

| **link**            | **destination** |
| ------------------- | --------------- |
| hamburger menu icon | home/nav open   |

### Home/nav open

| **link**        | **destination**    |
| --------------- | ------------------ |
| logo            | Home/nav-closed    |
| menu close icon | home/nav-closed    |
| pizza           | pizza/nav closed   |
| burgers         | burgers/nav closed |
| dessert         | dessert/nav closed |

### Pizza/nav closed

| **Header**          | **Header**     |
| ------------------- | -------------- |
| logo                | home/nav open  |
| hamburger menu icon | pizza/nav open |

### Pizza/nav open

| **link**        | **destination**    |
| --------------- | ------------------ |
| logo            | Home/nav-closed    |
| menu close icon | pizza/nav-closed   |
| pizza           | pizza/nav closed   |
| burgers         | burgers/nav closed |
| dessert         | dessert/nav closed |

### Burgers/nav closed

| **Header**          | **Header**       |
| ------------------- | ---------------- |
| logo                | home/nav open    |
| hamburger menu icon | burgers/nav open |

### Burgers/nav open

| **link**        | **destination**    |
| --------------- | ------------------ |
| logo            | Home/nav-closed    |
| menu close icon | burgers/nav-closed |
| pizza           | pizza/nav closed   |
| burgers         | burgers/nav closed |
| dessert         | dessert/nav closed |

### Dessert/nav closed

| **Header**          | **Header**       |
| ------------------- | ---------------- |
| logo                | home/nav open    |
| hamburger menu icon | dessert/nav open |

### Dessert/nav open

| **link**        | **destination**    |
| --------------- | ------------------ |
| logo            | Home/nav-closed    |
| menu close icon | dessert/nav-closed |
| pizza           | pizza/nav closed   |
| burgers         | burgers/nav closed |
| dessert         | dessert/nav closed |

### Testing

Use the play button at the top right of the screen to review your prototype. Test each interaction listed in the tables above. You are testing interactions and design.

#### Interaction testing

Make sure all interactions behave the way you expect. Check that the animations are all the same type. Every action should have a way to return to the original state. Make sure there is a way to get back to the home page.

#### Design testing

When you are testing, you may see some text or images _Jumping around_. This is caused by something not being properly aligned. Go back to the design view and fix the positioning of elements that are not correctly aligned.

## Sharing the prototype

Typically, you will want to share your prototypes with clients. To do this:

### Sharing for review

1. select the _Share_ button at the top of the screen
2. select _anyone with the link_ and _can view prototypes_
3. select _Copy link_
4. send reviewers the link

### Sharing for collaboration

1. select the _Share_ button at the top of the screen
2. enter an email address of the person you want to collaborate with
3. beside the email address, select _Can edit_
4. Select _Invite_
5. The person(s) will receive an email with instructions
6. A Figma account is required for collaboration
