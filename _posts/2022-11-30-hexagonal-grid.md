---
title: 'Hexagonal Grid'
date: 2022-11-30
permalink: /posts/2022/10/hexagonal-grid/
tags:
  - plt
  - implementation
  - hexagon
---

In this blog, I'll provide an implementation of a hexagonal grid.
The creation of the four different types of hexagonal grids is shown in the following figure.
I'll also show how to retrieve a grid cell's coordinates given a window coordinate in pixel space which is useful for mouse interaction.

The hexagonal paving is a tiling of the plane by regular hexagons.
It is one of the three existing tilings of the plane among the square paving and the triangular paving.
Compared to the square paving, the hexagonal paving has a more natural shape and is more aesthetically pleasing.


------

# The four different types of hexagonal grids



<table>
  <tr>
    <td>
      <figure>
        <img src="/images/hexagonal-grid/hexagon_grid_even-horizontal.svg" alt="even-horizontal">
      </figure>
    </td>
    <td>
      <figure>
        <img src="/images/hexagonal-grid/hexagon_grid_even-vertical.svg" alt="even-vertical">
      </figure>
    </td>
    <td>
      <figure>
        <img src="/images/hexagonal-grid/hexagon_grid_odd-horizontal.svg" alt="odd-horizontal">
      </figure>
    </td>
    <td>
      <figure>
        <img src="/images/hexagonal-grid/hexagon_grid_odd-vertical.svg" alt="odd-vertical">
      </figure>
    </td>
  </tr>
</table>

------

# 6 Triangle

The hexagonal grid is composed of 6 triangles.
The following figure shows the 6 triangles of a hexagon.

create markdown table next line

<table>
 <tr>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_flat.svg" alt="flat">
    </td>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_pointy.svg" alt="pointy">
    </td>
  </tr>
</table>

<table>
 <tr>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_even-horizontal.svg">
    </td>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_even-vertical.svg">
    </td>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_odd-horizontal.svg">
    </td>
    <td>
      <img src="/images/hexagonal-grid/hexagon_triangle_odd-vertical.svg">
    </td>
  </tr>

</table>


------

# Conclusion

This blog post introduces the hexagonal grid and the different types of hexagonal grids.
It also shows how to retrieve a grid cell's coordinates from a window coordinate.
The code for this blog post is available on GitHub.


------

# References

[1] https://en.wikipedia.org/wiki/Hexagonal_paving

[2] https://www.redblobgames.com/grids/hexagons/

=======