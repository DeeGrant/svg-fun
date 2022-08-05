# svg-fun

An attempt at playing with svgs. Inspired from [this](https://www.youtube.com/watch?v=9qen5CKjUe8) video.

## learning

- Commands (the letters)
  - uppercase are absolute commands (to a specific point on the canvas)
  - lowercase are relative commands (distances from the previous point)
  - Move: M
  - Line: L
  - Horizontal Line(shorthand): h
  - Vertical Line(shorthand): v
  - Cubic Bezier: C handle_point_1 handle_point_2 curve_endpoint
  - Smooth Curve To: S handle_point_1 endpoint
    - assumes the trajectory of the last bezier handle on previous input
  - Close the path?: Z
- Coordinates (the numbers)
- [good example of syntax](path_syntax_ex_5.svg)

### tips and tricks
- if all the commands are relative, changing the first coordinate translates the entire svg within the viewBox.

### issues
- depending on the line path syntax, the preview in webstorm is very pixelated. The actual svg is fine though.
- the style tag wasn't modifying the path tag. I had to use inline styling
