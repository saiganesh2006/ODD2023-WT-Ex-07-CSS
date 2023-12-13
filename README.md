## Ex-07-CSS

## AIM:
Using CSS media queries, modify the webpage's color scheme with the following requirements:
Default Color Scheme:
Background color: Light gray (#f4f4f4)
Text color: Dark gray (#333)
Link color: Blue (#007bff)
Small Screen Adaptation (Max-width: 600px):
## Objective 1:
## Using CSS media queries to modify the webpage's color scheme.

## Step-1:

The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."

## Step-2:

The default color scheme for the webpage is defined in the body and a (anchor) styles. The background color is set to a light gray (#f4f4f4), text color is set to dark gray (#333), and anchor links are set to a blue color (#007bff).

## Step-3:

A media query is used to adjust the color scheme for small screens (max-width: 600px).On small screens, the background becomes dark (#333), text color becomes light (#f4f4f4), and anchor links turn green (#28a745).Media Query for Dark Mode Preference:

## Step-4
Another media query is used to check if the user prefers a dark color scheme.In dark mode, the background becomes black (#000), text color becomes white (#fff), and anchor links turn a teal color (#17a2b8).

## Step-5:

The <body> section contains two heading elements and an anchor link .The headings are for displaying information, and the anchor link is an example to demonstrate the color change on different screen sizes and preferences.

## Step-6:
Testing:
You can test the behavior by resizing the browser window to see the color scheme changes for small screens.If your system has dark mode preference enabled, the dark color scheme should be applied.
## CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Color Scheme</title>

  <style>
/* Default Color Scheme */
body {
  background-color: #f4f4f4;
  color: #333;
}

a {
  color: #007bff;
}

/* Small Screen Adaptation */
@media (max-width: 600px) {
  body {
    background-color: #333;
    color: #f4f4f4;
  }

  a {
    color: #28a745;
  }
}

/* Dark Mode Preference */
@media (prefers-color-scheme: dark) {
  body {
    background-color: #000;
    color: #fff;
  }

  a {
    color: #17a2b8;
  }
}
  </style>
</head>

<body>
  <h1>Using CSS MEDIA QUERIES to modify the webpage's color scheme.</h1>
  <h2>Welcome to Sai Ganesh Webpage..!</h2>

  <!-- Link to demonstrate blue color -->
  <a href="www.saveetha.ac.in">SAVEETHA.COM</a>
</body>

</html>
```

## OUTPUT:
# If the user set the device in Light Mode:
![Screenshot 2023-12-13 103838](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/4c664514-ec21-44ea-a4ea-2189046d9932)

# If the user set the device in Dark Mode:
![image](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/56629fda-2ce4-430b-9468-99e9cfadd7bb)

## Objective 2:
## Using CSS media queries to modify mobile and desktop styles.

## Step-1:
HTML Structure:
The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."

## Step-2:
CSS Styles:
The CSS styles are defined inside a <style> tag in the <head> section.Styles for desktop devices are defined initially, setting the font size, background color, and text color for the body. A container class is defined for styling a central content container with a maximum width, padding, background color, border, and box shadow.Class selectors like .container, .device-specific, and .device-specific2 are used to target specific HTML elements for styling.

## Step-3:
Media Query for Mobile Devices:
A media query (@media screen and (max-width: 599px)) is used to apply different styles for mobile devices with a width less than 600px.Inside the media query, the font size, background color, and text color for the body are adjusted for smaller screens.The styles for the .container class are modified, reducing padding, changing the background color, removing the box shadow, and adjusting the border.Two additional classes, .device-specific and .device-specific2, are defined with specific styles (bold and different colors) to demonstrate how styles can be tailored for mobile devices.

## Step-4:
To observe the responsive design, you can resize the browser window or use a developer tool to simulate different device widths.Notice how the styles change when the screen width is less than 600px, reflecting a mobile-friendly design.

## Step-5:
Testing:
To observe the responsive design, you can resize the browser window or use a developer tool to simulate different device widths.Notice how the styles change when the screen width is less than 600px, reflecting a mobile-friendly design.
## CODE:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Styles for desktop devices */
    body {
      font-size: 16px;
      background-color: #f2f2f2;
      color: #333;
    }

    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border: 1px solid #ddd;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    /* Media query for mobile devices with width less than 600px */
    @media screen and (max-width: 599px) {
      body {
        font-size: 14px;
        background-color: #e6e6e6;
        color: #555;
      }

      .container {
        padding: 10px;
        background-color: #f9f9f9;
        border: 1px solid #ccc;
        box-shadow: none;
      }

      .device-specific {
        font-weight: bold;
        color: #ff5733;
      }
      .device-specific2 {
        font-weight: bold;
        color:blue;
      }
    }
  </style>
  <title>Responsive Design Example</title>
</head>
<body>
  <div class="container">
    <h1>Responsive Design Example</h1>
    <p>This is some text that will be visible on all devices. The background color and font size will change based on the screen width.</p>
    <p class="device-specific">This text will have different styles on different devices. It's now bold and has a different color on mobile devices.</p>
    <h2 class="device-specific2">Welcome to Sai Ganesh Webpage..!</h2>
  </div>
</body>
</html>


```
## OUTPUT:
# If the user was using the large screens like laptops,pc's:
-![Screenshot 2023-12-13 105048](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/b6f1e5db-f5e8-4783-a642-8bf5d4f8196a)

# If the user was using the small screens like mobile:
![WhatsApp Image 2023-12-13 at 10 52 30_74b09348](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/6230db2e-e4c3-4a1e-95db-876085e3db91)

## Ojective 3:
## Using CSS media queries to represent orientation scheme.

## Step-1:

The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."

## Step-2:
CSS Styles:
The CSS styles are defined inside a <style> tag in the <head> section.Two media queries (@media (orientation: portrait) and @media (orientation: landscape)) are used to apply different styles based on the orientation of the device.

## Step-3:
Portrait Orientation Styles:
Inside the @media (orientation: portrait) query, the background color of the body is set to a light blue (#e6f7ff). This will be applied when the device is in portrait orientation.
Landscape Orientation Styles:
Inside the @media (orientation: landscape) query, the background color of the body is set to a light purple (rebeccapurple). This will be applied when the device is in landscape orientation.

## Step-4:
Orientation Media Queries:
The orientation media query is used to check whether the device is in portrait or landscape orientation.When the device is in portrait mode, the styles within @media (orientation: portrait) are applied.When the device is in landscape mode, the styles within @media (orientation: landscape) are applied.

## Step-5:
Testing:
To observe the changes based on orientation, you can view the webpage on a device with the capability to change orientations (such as a smartphone or tablet) or use a browser's developer tools to simulate different orientations.
## CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Orientation Scheme</title>

  <style>
/* Styles for portrait orientation */
@media (orientation: portrait) {
  body {
    background-color: #e6f7ff; /* Light blue background for portrait orientation */
  }

}

/* Styles for landscape orientation */
@media (orientation: landscape) {
  body {
    background-color: rebeccapurple; /* Light red background for landscape orientation */
  }

}

  </style>
</head>

<body>
  <h1>Orientation based on media curies</h1>
  <h2>Wwelcome to Sai Ganesh Web page..!</h2>


</body>

</html>
```
## OUTPUT:
# Webpage's background colour is purple when opened on landscape orientation (pc):
![image](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/474679fa-6a86-4c50-aeda-01c642cd073a)
# Webpage's background colour changes to light green when opened on portriat orientation (mobile phone):
![WhatsApp Image 2023-12-13 at 11 05 33_16393f64](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/7ed6507e-5e04-4368-91f4-327c47ef9101)

## Objective 4:
## Responsive Typography using CSS Media queries

## Step-1:
The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."

## Step-2:
CSS Styles:
The CSS styles are defined inside a <style> tag in the <head> section.Default styles for all devices are specified, including a base font size of 16px, a line height of 1.6, and a margin of 20px for the body.

## Step-3:
Media Queries:
There are two media queries used to make the typography responsive to different screen widths:
The first media query (@media screen and (min-width: 600px) and (max-width: 899px)) targets devices with a width between 600px and 899px. It adjusts the font size to 18px and the line height to 1.5 for the body.
The second media query (@media screen and (min-width: 900px)) targets devices with a width of 900px and above. It adjusts the font size to 20px and the line height to 1.4 for the body.

## Step-4:
Responsive Typography:
The responsive typography is achieved by using media queries to adjust the font size and line height based on the screen width.As the screen width changes, the font size and line height of the text in the body will dynamically adapt to provide a better reading experience on different devices.

## Step-5:
Testing:
You can test the responsiveness of the typography by resizing the browser window or using browser developer tools to simulate different device widths.Observe how the font size and line height change according to the specified media query conditions.

## CODE:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Default styles for all devices */
    body {
      font-size: 16px;
      line-height: 1.6;
      margin: 20px;
    }

    /* Media query for devices with width between 600px and 899px */
    @media screen and (min-width: 600px) and (max-width: 899px) {
      body {
        font-size: 18px;
        line-height: 1.5;
      }
    }

    /* Media query for devices with width 900px and above */
    @media screen and (min-width: 900px) {
      body {
        font-size: 20px;
        line-height: 1.4;
      }
    }
  </style>
  <title>Responsive Typography Example</title>
</head>
<body>
  <h1>Responsive Typography Example</h1>
  <p>
    This is some text on the webpage. The font size and line spacing will adjust based on the screen width.
  </p>
 <h2>Welcome to Sai Ganesh Webpage..!</h2>
</body>
</html>
```
## OUTPUT:
# If the user open it larger devices like pc
![Screenshot 2023-12-13 112553](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/1d0c25ef-8b3f-47c8-944e-becd7e701a1c)
# If user open it in mobile phones
![WhatsApp Image 2023-12-13 at 11 36 15_48b18792](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/65398b05-1c86-41e2-ac3b-d03eba7d9f4e)

## Objective 5:
## Print-friendly styles for web pages using CSS media quries

## Step-1:
The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."
## Step-2:
CSS Styles:
The CSS styles are defined inside a <style> tag in the <head> section.Default styles for the webpage are specified, including a light gray background for the body, dark gray text color, and a blue color for links.
Non-Essential Element Styling:
The class .non-essential is defined with a display: block; property, making elements with this class visible by default.

## Step-3:
Media Query for Print Styles:
A media query (@media print) is used to define styles specifically for printing.Inside the print media query, background color, text color, and link color are adjusted to be more suitable for printing (white background, black text, and cyan links).The .non-essential class has a display: none; property within the print media query, hiding non-essential elements when printing.

## Step-4:
Print-friendly Styles:
The purpose of this code is to provide a print-friendly version of the webpage by adjusting styles when the page is printed.The print styles are designed to optimize the content for a printed document, with changes to background color, text color, link color, and the visibility of non-essential elements.

## Step-5:
Testing Print Styles:
You can test the print-friendly styles by using the browser's print functionality or a print preview. Observe how the styles change when preparing to print the webpage.

## CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Print-friendly Styles</title>

  <style>
    /* Default styles for the webpage */
    body {
      background-color: #f4f4f4; /* Light gray background */
      color: #333; /* Dark gray text color */
    }

    a {
      color: #007bff; /* Blue link color */
    }

    .non-essential {
      display: block; /* Visible by default */
    }

    /* Media query for print styles */
    @media print {
      body {
        background-color: #fff; /* White background for printing */
        color: #000; /* Black text color for printing */
      }

      a {
        color: #17a2b8; /* Cyan link color for printing */
      }

      .non-essential {
        display: none; /* Hide non-essential elements for printing */
      }

    }
  </style>
</head>

<body>
  <h1>Print-friendly Styles Example</h1>
  <p>This is the content of your webpage.</p>
  <p class="non-essential">This is a non-essential element.</p>
  <h2>Welcome to Sai Ganesh webpage..!</h2>
</body>

</html>
```

## OUTPUT:
# When we open webpage in view-mode:
![image](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/afc0e0f8-da06-4f9b-9ca7-24fc3a4757a8)
# When we set to get print of webpage:
![image](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/d3961b29-b1b3-4f17-8e4f-96364cca63d0)

# Objective 6:
# Dark mode Implementation using CSS media queries

## Step-1:
The HTML document starts with the usual <!DOCTYPE html> declaration.The <html> tag specifies the language as English (lang="en").The <head> section includes meta tags for character set and viewport settings.
The title of the webpage is set to "Color Scheme."

## Step-2:
CSS Styles:
The CSS styles are defined inside a <style> tag in the <head> section.Default styles for the webpage are specified, including a light gray background for the body and dark gray text color.

## Step-3:
Dark Mode Media Query:
A media query (@media (prefers-color-scheme: dark)) is used to detect the user's system preference for dark mode.Inside the dark mode media query, background color and text color are adjusted to create a dark mode appearance (black background and white text).

## Step-4
Adaptive Color Scheme:
The purpose of this code is to create an adaptive color scheme that changes based on the user's system preference for dark mode.The default color scheme is set, and if the user has a preference for dark mode, the styles inside the dark mode media query are applied.

## Step-5:
Testing Dark Mode:
You can test the dark mode by toggling your system's dark mode setting (if your system supports it). Alternatively, you can use browser developer tools to simulate a dark mode preference.Observe how the color scheme of the webpage changes when dark mode is enabled.

## CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Mode Example</title>

  <style>
    /* Default color scheme for light mode */
    body {
      background-color: #f4f4f4; /* Light gray background */
      color: #333; /* Dark gray text color */
    }

    /* Additional styles for light mode as needed */

    /* Dark mode preference */
    @media (prefers-color-scheme: dark) {
      body {
        background-color: #000; /* Dark background for dark mode */
        color: #fff; /* Light text color for dark mode */
      }

    }
  </style>
</head>

<body>
  <h1>Dark Mode Example</h1>
  <p>This webpage dynamically adapts to the user's system preference for dark mode.</p>
  <p>Toggle your system's dark mode setting to see the changes!</p>
  <h2>Welcome to Sai Ganesh Webpage..!</h2>
</body>

</html>
```

## OUTPUT:
# Webpage is Displayed in light mode when device is running on light theme
![image](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/fc740a1a-2799-40fb-8732-975998e79b32)

# Webpage is Displayed in dark mode when deivce is running on dark mode
![Screenshot 2023-12-13 151701](https://github.com/saiganesh2006/ODD2023-WT-Ex-07-CSS/assets/145742342/5588efcd-8925-4813-bf7d-e65605bd4366)

## RESULT:
Therefore, functionalities of CSS media queries are clearly demonstrated using examples for each type.

## DEVELOPED BY: D.B.V.SAI GANESH
## REGISTER NUMBER: 212223240025
