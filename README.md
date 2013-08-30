# Browser Click Loss Test

While working on a project that involved frequent DOM manipulation, I observed mouse click events being lost. When a click event handler is registered on a parent, and a click happens on a child, then the parent should normally receive the click event. However, if the child element is replaced at exactly the wrong time, the click event is lost.

This test demonstrates this issue. The problem is much worse on Chrome, but rapidly becomes visible on Firefox as the DOM replacement rate increases.
