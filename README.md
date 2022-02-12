# Discord - Clone Challenge

## Overview

My attempt at cloning the Discord landing page. If time permits, I will also try to clone the Download and Help pages, but with reduced design and greatly-reduced functionality.

## Design Process

Here I will make note of my initial guesses at how to achieve the desired layout. I will also write any issues I come across, as well as how I overcame those issues. Since CSS still feels very unpredictable to me, I feel this will help me immensely.

### Landing Page

#### Navigation

The first element on the landing page (and others, though in different, inconsistent forms) is the Navigation elements. This consists of the Discord logo (a controller-type icon and a stylized 'Discord' text), 6 navigation links (Download, Nitro, Safety, Support, Blog, and Careers) and an 'Open Discord' button.

At a glance, I can imagine this navigation can be achieved by wrapping all three main elements in a flex container, and justifying them with 'space-between'. The 6 navigation links can also be inside a flex container, with a small 'gap' separating them.

On smaller screens, the navigation turns into a hamburger menu. I will probably skip this behavior.

#### Hero Section

The next element is the 'Hero' section. On desktop displays, it appears to have three main elements inside of a grid or flex container.

- h1 with an introductory text
- div or p element with a short write-up
- div that serves as a flex container for two buttons
  - 'Download for Windows' button
  - 'Open Discord in your browser' button

This section appears to change layouts at 4 or more breakpoints. To be honest, some of the changes are a littel disorienting and inconsistent feeling, so I may use a simple flexbox that has a flex-wrap of wrap to achieve this layout.

The background of this section is a series of three different illustrations, which tie together in different layouts as the screen size changes. I may simplify this design aspect to begin with.

#### 'Invite-Only

The third section is rather straightforward. It consists of an illustration, a header, and a short paragraph. At full screen, the header / paragraph are aligned in a column on the right 40%'ish side of the section, and the illustration is in the left column. At smaller screens, the 2-column layout chagnes into a 1-column layout, with the illustration on top (so a flex-wrap of wrap-reverse?)

#### 'Hanging Out' Section

The fourth section is similar to the previous one. The illustration, header, and paragraph have different content (obviously), and the illustration is in the right column instead of the left.

#### 'Community' Section

The fift section is similar to the previous one. The illustration, header, and paragraph have different content (obviously), and the illustration is in the left column instead of the right.

#### 'Reliable Tech' Section

The sixth section again consists of a header, paragraph, and illustration. This time, the text and illustration are aligned in a one-column layout at desktop sizes. This layout persists as the screen gets smaller.

#### Footer

A grid (could use flex?) container with two other containers.

On smaller screens:

- Container with 'Imagine a place', USA flag / 'English, USA' text, and social media buttons for Twitter, Instagram, Facebook and Youtube
- A 2x2 series of links, with headings for each category: 'Product', 'Company', 'Resources', and 'Policies'
  - Each of these categories contains 3 or more links
- The first container and second container are aligned in a single column

On bigger screens:

- The first container and second container are aligned side-by-side in a 2-column layout

#### Buttons

There are four Buttons on the landing page. All these buttons share the same rounded design and the same hover effect (a box-shadow appears)

#### Navigation Links

The 6 navigational links share the same styling, with a simple bottom border appearing below them when they are hovered over.
