# hover-move
  Nice display of additional information on hover. Native javaScript. Similar to hoverdir - jQuery plugin.
  
  - preview https://codepen.io/vitalij-nikitenko/pen/JjELBmL

to get started:

```
import HoverMove from "./hover-move";

const containers = document.querySelectorAll(`.hover__container`);

containers.forEach((container) => {
const hoverMove = new HoverMove(container, `.hover__description`);
    hoverMove.init();
});
```

- hover__container - for example an element Li
- hover__description - movable element selector inside hover__container

css example:

```
.hover__container {
  position: relative;
  overflow: hidden;
}

.hover__description {
  position: absolute;
  top: auto;
  left: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  background-color: $you-color;
  transition: .3s ease;
  pointer-events: none;
}

```
