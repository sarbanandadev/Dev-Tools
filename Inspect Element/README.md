# HOW TO USE WEB DEVELOPER CONSOLE ON MOBILE BROWSER

There might be many reasons to use developer console on your phone, maybe you need to run JavaScript on your browser console, to inspect elements and check style properties. Your reason to use developer console is up to you and the mobile browser by default doesn't support developer tools like console and inspect element.

If you are using Chrome on your smartphone there is a way to [use the developer console remotely by connecting your phone to a PC and by remote debugging](https://developers.google.com/web/tools/chrome-devtools/remote-debugging?hl=en).

But what if you want to use your web developer console on your smartphone itself without any PC. 
Yes, it is possible using a simple tool called [Eruda](https://github.com/liriliri/eruda).

So let's setup Eruda on our browser to open browser console for any website.

| ![Console](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/console.jpg) |
| --- |
| [Console](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/console.jpg) |

## Steps to use browser console on phone without PC
1. Open your phone browser( Chrome is preferred).
2. Select Bookmarks.
3. Edit any unwanted bookmark.
4. In Name type Inspect Element.
5. In URL paste the code below.

```
javascript:(function () { var script = document.createElement('script'); script.src="//cdn.jsdelivr.net/npm/eruda"; document.body.appendChild(script); script.onload = function () { eruda.init() } })();
```

| ![Bookmarks](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/bookmark.jpg) |
| --- |
| [Bookmarks](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/bookmark.jpg) |

6. Save the Bookmark.
7. Go to any site you want to use browser console.
8. After the site is completely loaded, `Type Inspect Element on the address bar` and select the address we just bookmarked.

| ![Search](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/search.jpg) |
| --- |
| [Search](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/search.jpg) |

9. Now you will `see an icon appear right on your web page`. Click on it to open web developer console tools.

| ![Button](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/button.jpg) |
| --- |
| [Button](https://github.com/sarbanandadev/Dev-Tools/blob/sarbananda/Inspect%20Element/button.jpg) |

## Conclusion
This is the simplest method to use web developer console on your mobile browser and run some JavaScript code on any website. Some website does not allow to run external JavaScript on their site through phones but you can try and check.

If your aim is to run JavaScript on a website you can use `javascript:<<code>>` on the address bar. You can also directly paste the code given above to open developer tools but when you paste it directly into your address bar, the beginning part `javascript:` will not be pasted so you need to type it in for the code to work.
