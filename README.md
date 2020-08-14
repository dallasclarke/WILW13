# What I learned Week-13.

## CSS Flex

- Below defines a flex container and enables flex content for all direct children.

  . container {
  display: flex;
  }

  - *flex-direction* Establishes the main axis defining the direction of items that are in the flex container.
  
  flex-direction: row | row-reverse | column | column-reverse
  

- *justify-content:* Aligns items along main axis.  Also helps distributing the extra space leftover and places some controls over the alignment when overflown.
  
  justify-content: flex-start | flex-end | center | space-betwen | space-around | space-evenly

  - *align-items:* Defines behavior for how items are laid out along the cross axis.

    align-items: stretch | flex-start | flex-end | center | baseline

    - *align-content* Aligns containers lines within when there is extra space in the cross axis.

    align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch

    - *flex-grow* Has the ability to grow flex item if necessary. It will take in a unitless value and it dictates what amount of space the container should take up.

    flex-grow: 3;

    - *flex-shrink:* Does the opposite of flex-grow.


## CSS Grid

- Below defines the element as a grid container making a new grid format context for contents.

.container {
    display: grid;
}

- *grid-template-columns:* and *grid-template-rows:* This defines the columns and rows of the grid. The values represent the track size and space between them reps the grid line.

Values:

- track-size - length, percentage or a fraction of the space in the grid. **Ex.** 1fr, 25px, 30%
- line-name - Arbitrary name of choosing.

- *grid-template-areas:* A grid template that references the names of grid areas which are specified with the *grid-area* property. Repeating the names of a grid are will cause contents to span to those cells.

*ex.* grid-template-areas: hdr hdr hdr;
      grid-area: hdr;

      