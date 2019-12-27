Notes to cover the web design for Assignment 2
PART 1:
Website archive can be found in this file in the folder names “HaukaiRestaurant”
Copy of the READ ME file for ease of reading

My GitHub website address:
https://eduworldz.github.io/HaukaiRestaurant.github.io/
Part 1(c): Accessibility Guidelines used: I have followed Web Content Accessibility Guidelines (WCAG) 2.0 created by the W3C organisation as best as I can see using:

- Easy to follow and understandable language.
- Making it easier for screen readers by using header tags (hi, h2 and h3).
- Using html elements for pages layouts (header, nav, main, footer) to divide the page elements.
- Text alternatives for photos (Alt tags) for the visually impaired on images.

Tests completed on various validation services with screenshots of the website passing these test in this folder.

1.(d) Privacy statement has been added to the website and accessible from the link on the pages that use forms to collect data (contact.html and reservations.html) and also copied onto a text file in this file folder headed “Privacy Statement”.

1.(e) There are security issues when embedding Flash, Java Applets, videos, sound files, images or PDF files into the website as these files can be hacked or altered by the original owners at any time in the future and thus affect users of the website being designed. External website linked to can also not be relied upon as you do not know the level of security they use to protect their content.

Another safeguard is to use HTTPS on the site to ensure that information passed between the users  browser and the website is secure.

Also ensure that all information collected though the website on users is secure. Use the CIA Security  Model: Files should only access and modified by people on the appropriate access lists and available to specified people whenever they require access. Web developers should also be up to date with the Open Web Application Security Project (OWASP) and associated risks.

A major risk is Denial of Service attacks. These hackers will bombard the server of your website with large numbers of HTTP requests that deny legitimate visitors access to the web application. Rather that opting for a larger server to handle more requests, it is more common to use a content delivery network (CDN). A CDN is a globally distributed set of servers that keep copies of websites and deliver them from the closest CDN server to a user. This increases security and performance. The HTTP caching keeps the CDN server copies up to date and tracks any changes to the original website.

PART 2

b.	Applying responsive design principles:
I tested the website as I was making it and committing to my Git to ensure it met requirements for various devices and screen sizes. Methods I used were for the resizing on images by CSS to set the maximum width to a percentage instead of a set size. This allows the content to resize depending on the screen size used. Using “auto” on the height allowed the height to alter in proportion to the width:

.responsive {
      max-width: 100%;
      height: auto;
    }

I used the same feature on the .col-container and .column CSS for the columns used to place the image and static text on the home page and for the dynamic content of the map and google contact form  on the contact page. Therefore there is no need to scroll the screen horizontally to view all the content.

I also use the variable width (.vw) extension on the font size and padding in the header to ensure the size and font alter automatically to fit screen sizes.

c.	“Trailing Spaces” extension:
Installed and tested with this example showing 3 examples on lines 33, 43 and 48 on the CSS page

d.	Optimising the page loading time:
In order to be able to test it for 2G I had to create a custom “throttling” option that fits the specifications of 250 kbs download, 50 kbs upload, and 300 ms latency.

