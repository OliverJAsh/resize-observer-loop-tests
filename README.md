# `ResizeObserver` loop tests

References:

-   The best explanation of this problem: https://webkit.org/blog/9997/resizeobserver-in-webkit/#:~:text=observation.-,How%20Observations%20are%20Delivered
-   https://developer.mozilla.org/en-US/docs/Web/API/ResizeObserver
-   https://www.w3.org/TR/resize-observer/#:~:text=loop.-,Infinite%20loop%20is%20prevented,An,-error

The error message in different browsers:

-   Chrome: "ResizeObserver loop limit exceeded"
-   Safari and probably others: "ResizeObserver loop completed with undelivered notifications"

Note: in Chrome, these errors are never logged to the console but they are received by `window.onerror`.
