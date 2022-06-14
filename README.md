# Beanie Babies

This is Project Zero on the journey to learning web development!

View demo: https://whimsical-jelly-692e94.netlify.app/

This demo was written after going through W3Schools HTML and CSS sections. As such, its purpose was to practice various interesting aspects of HTML and CSS that I found interesting, and so I purposely avoided using any JavaScript. Specific details on what I did can be found in the comments.

Here are concepts new to me that I attempted to implement:

- Mobile-first design: When making websites in the past, I've always designed them to work on desktop since I'm the only one who uses it, and I rarely use mobile. So this is the first design that I've taken the mobile-first approach, which is design it first with mobile screens in mind, and adapt for larger screens afterwards.
- CSS reset
- Linear gradients
- Math calculations (calc and min) in CSS
- Flexbox
- Transitions, including those on hover, and the differences in using display, visibility, and opacity properties to hide and show elements
- Up and down arrows using CSS borders and rotation
- Multiple transforms
- Animations
- CSS Lint for syntax checking
  - Values of 0 should not have units specified; however, on further research it seems that this can break calculations and make it more difficult to use some developer tools
  - \* is slow; however, on further research, this may not be the case.
- Lighthouse for performance checking: Received a performance rating of 78 due to speed and large size of content to be delivered.

  - Learned about next-gen image formats AVIF and WebP
  - Caching of static assets (in this case, I just ignores this because I'm using some images from another site)
  - Eliminating render-blocking resources by deferring non-critical CSS, learning about optimizing the Critical Rendering Path and improving First Contentful Paint (FCP), including asynchronously loading non-critical CSS files (technically uses some JavaScript but I let this go)
  - Add meta description for SEO
  - The rendering pipeline, Cumulative Layout Shift (CLS): 4 things a browser can animate cheaply are position, scale, rotation, and opacity. In my page, I am animating length changes of my boxes and so I will cause a Cumulative Layout Shift. What this suggests is that instead of animating a length change to display additional information, I should perhaps create a modal/popup to display additional information that doesn't cause a CLS.

All in all, I learned a lot from this project, especially with Lighthouse. I did a Lighthouse on another page that I created (I knew it was terrible), and scored at 25! It's good to see what's wrong and how to fix it for the future. I'll aspire to make things more efficient.
