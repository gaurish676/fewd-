# Front End Web-Development Project

Explaining the HTML and CSS Code for a Simple Portfolio Webpage
This code consists of two main files: an HTML file and a CSS file. The HTML file provides the structure and content of the webpage, while the CSS file is used to style the webpage. Let's break down each file and understand its purpose and functionality.

HTML Structure
The HTML code defines the content and layout of the portfolio webpage.

Document Declaration and Meta Information

//html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>your portfolio</title>
</head>
The <!DOCTYPE html> declaration specifies that this is an HTML5 document.
The <html> element encloses the entire HTML document, and the lang="en" attribute specifies that the content is in English.
The <head> section contains meta-information like the character set (UTF-8), viewport settings for responsive design (width=device-width, initial-scale=1.0), and links to external resources such as the CSS stylesheet (styles.css).
The <title> tag defines the name of the webpage displayed in the browser tab.
Body of the Document

html

<body>
    <header>
        <h1>Gaurish Bangera</h1>
    </header>
    <main>
        <section class="profile">
            <div class="photo">
                <img src="your-photo.jpg" alt="Your Photo">
            </div>
            <div class="bio">
                <h2>About myself</h2>
                <p></p>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 Gaurish Bangera All rights are reserved</p>
    </footer>
</body>
<pre>The <body> element contains the visible content of the webpage.

Inside the <body>, there are three main sections: header, main, and footer.

Header: The <header> section contains the name of the individual (<h1>Gaurish Bangera</h1>), which serves as the webpage’s title.
Main: The <main> section is where the primary content of the portfolio resides. It contains:
A profile section with two sub-elements:
Photo: A <div> containing an <img> tag to display a profile picture (the src="your-photo.jpg" is a placeholder for the actual photo file).
Bio: A <div> with an <h2> for the heading "About me" and a <p> tag where the user can describe themselves.
Footer: The <footer> section provides a copyright notice (&copy; 2023 Gaurish Bangera).
CSS Styling
The styles.css file is used to style the HTML elements defined above. It ensures that the portfolio page is visually appealing and responsive.

Global Styling

css

body, h1, h2, p {
    margin: 0;
    padding: 0;
}
This code removes default margins and padding for the body, h1, h2, and p elements, ensuring that the layout starts from a clean slate.
Body Styling

css

body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.6;
}
The body of the page is styled with a sans-serif font family (Arial, Helvetica, sans-serif), making the text more modern and easy to read.
The line-height is set to 1.6 to improve the readability of the text by giving it more space between lines.
Header Styling

css

header {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem;
}
The header element has a dark background color (#333) with white text (#fff), giving it a high contrast and clean look.
The text is centered (text-align: center), and padding: 1rem ensures some space around the content inside the header.
Main Section Styling

css

main {
    padding: 2rem;
}
The main section is given 2rem of padding to ensure that the content does not touch the edges of the screen and has adequate space around it.
Profile Section Layout

css

.profile {
    display: flex;
    align-items: center;
}
The .profile class uses display: flex to create a flexible layout, where the photo and bio are aligned horizontally.
align-items: center ensures that both the image and bio text are vertically centered.
Photo Styling

css

.photo {
    flex: 1;
    padding: 0 2rem;
}
.photo img {
    max-width: 100%;
    height: auto;
    border-radius: 50%;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}
The .photo class ensures that the image takes up a flexible portion of the layout (flex: 1).
The image itself is styled to have a circular shape (border-radius: 50%) with a subtle shadow (box-shadow: 0 0 10px rgba(0, 0, 0, 0.2)) to make it visually stand out.
Bio Section Styling

css

.bio {
    flex: 2;
}
The .bio class takes up more space than the photo (flex: 2), allowing more room for the text content.
Footer Styling

css

footer {
    text-align: center;
    padding: 1rem 0;
    background-color: #333;
    color: #fff;
}
The footer is styled similarly to the header, with a dark background (#333) and white text (#fff), creating visual consistency across the webpage.
The text-align: center and padding: 1rem 0 ensure that the footer content is centered and has some space around it.
Media Query for Responsiveness
css

@media screen and (max-width: 768px) {
    
}</pre>
<pre>This is a media query, which allows the website to adjust its layout based on the screen size.
The max-width: 768px condition targets devices with screen widths of 768px or less, such as tablets or smartphones.
Although the body of the media query is empty in this code, it can be used to add styles that improve the layout and user experience on smaller screens (e.g., adjusting font size, rearranging elements).
Conclusion
This simple portfolio webpage consists of a clean, responsive layout using HTML and CSS. The structure is basic but effective for displaying a personal portfolio, with clear sections for the header, profile image, bio, and footer. The use of flexbox allows for an adaptable and organized layout, and the CSS ensures that the design looks great on all devices with the help of a media query.

This layout can serve as a foundation for more advanced features and styling as the portfolio evolves, such as adding links, projects, or contact information.</pre>
