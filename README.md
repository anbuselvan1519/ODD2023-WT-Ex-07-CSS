# Ex-07-CSS
## Name: Anbuselvan.S
## Reference No: 23005959
### Ex-07(i)-CSS-Modify the webpage's color scheme
## AIM:
Using CSS media queries, modify the webpage's color scheme with the following requirements:

Default Color Scheme: Background color: Light gray (#f4f4f4) Text color: Dark gray (#333) Link color: Blue (#007bff) Small Screen Adaptation (Max-width: 600px):

Change the background color to dark gray (#333) Change the text color to light gray (#f4f4f4) Change the link color to light green (#28a745)

Dark Mode Preference:

If the user has set their device to dark mode, override the above styles with the following: Background color: Black (#000) Text color: White (#fff) Link color: Cyan (#17a2b8)

## DESIGN STEPS:(i)
### Step 1:
Start Define the document type as HTML.

### Step 2:
Open the HTML structure with the necessary head and body sections. In the head section, set the title of the webpage and define the styles for the webpage. The styles include: -->Default color scheme for the webpage. -->Adaptations for small screen sizes. -->Adaptations for users who prefer a dark color scheme.

### Step 3:
In the body section, create a division with the text “Saveetha Engineering College”. Also in the body section, create a list with links to the SEC Home Page, My Camnu, and GitHub.

### Step 4:
Close the HTML structure.

## CODE:(i)
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
   
    

    
    <style>
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
    <h1>Web Application Development</h1>
    <p><a href="http://lms.ai.saveetha.ac.in">MOODLE FOR AI</a></p>
    <h5>
        Web application development describes the process of designing, building, testing and deploying web-based applications that will be installed on remote servers and delivered to users or customers via the internet.
    </h5>
</body>
</html>
```
## OUTPUT:(i)
![WhatsApp Image 2023-12-26 at 19 41 49_f1a806f5](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/6a233d0d-9e28-4d19-94bc-1ffebf3b84ed)
![WhatsApp Image 2023-12-26 at 19 41 08_3b0e5487](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/99c47d5f-f855-45dc-925b-526efdf3f76e)
![WhatsApp Image 2023-12-26 at 19 41 36_99a2a2dd](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/97c7e1f0-0223-4d3b-af7f-c2b9de54a3cc)

### Ex-07(ii)-CSS-Different styles to a webpage.
## AIM:
To use a media query in CSS to apply different styles to a webpage for mobile devices (with widths less than 600px) and desktop devices (with widths greater than or equal to 600px) by providing an example CSS snippet to demonstrate your answer.

## DESIGN STEPS:(ii)
### Step 1:
Start the HTML document and create the root element.

### Step 2:
Inside , create the element and include a <style> element for CSS rules.

### Step 3:
Define CSS rules for desktop devices. Use a media query to define CSS rules for mobile devices.

### Step 4:
Inside , create a for the heading and an for the hyperlink.

## CODE:9(ii)
```
<!DOCTYPE html>
<htm>
  <head>
    <style type="text/css">
      
/* Styles for all devices (common styles) */

/* Mobile Devices (width less than 600px) */
@media only screen and (max-width: 599px) {
    /* Styles specific to mobile devices go here */
    body {
      font-size: 16px;   /* Adjust font size for better mobile readability */

      background-color: rgb(176, 204, 179);
      font-family: 'Times New Roman', Times, serif;
    }
  
    /* Additional styles for mobile devices */
  }
  
  /* Desktop Devices (width greater than or equal to 600px) */
  @media only screen and (min-width: 600px) {
    /* Styles specific to desktop devices go here */
    body {
      font-size: 25px; /* Adjust font size for better desktop readability */
      background-color: rgb(176, 204, 179);
      font-family: cursive;
    }
  
    /* Additional styles for desktop devices */
  }


    </style>
  </head>
</htm>


<body>
    <h1>Web Application Development</h1>
    <p><a href="http://lms.ai.saveetha.ac.in/my/">MOODLE FOR AI</a></p>
    <h5>
        Web application development describes the process of designing, building, testing and deploying web-based applications
         that will be installed on remote servers and delivered to users or customers via the internet.
    </h5>
</body>
</html>
```
## OUTPUT:(ii)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/747c22d7-2cb6-4c43-aed1-c8987faaa334)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/7432d27e-658c-4a36-82cd-dc1bf1e79e18)

### Ex-07(iii)-CSS Orientation-based Media Query
## AIM:
To explain how you can use CSS media queries to apply different styles based on the orientation (landscape or portrait) of the device. Provide a CSS example where you change the background color of the body based on the orientation.

## DESIGN STEPS:(iii)
### Step 1:
Identify the section in your HTML file where you want to add the CSS. This is typically within the <style> tags in the section.

### Step 2:
Define a CSS media query for each orientation. The syntax for a media query is @media (orientation: value), where value can be either portrait or landscape.

### Step 3:
Within each media query, specify the CSS rules you want to apply. In this case, you want to change the background color of the body.

### Step 4:
Close the media query with a }

### Step 5:
Close the media query with a }

### Step 6:
Save your HTML file.

## CODE:(iii)
```
<!DOCTYPE html>
<html>
  <head>
    <style type="text/css">
      
@media (orientation: portrait) {
    body {
      font-size:16px;
      background-color: rgb(232, 169, 169);
    }
  
    /* Add more styles for portrait orientation as needed */
  }
  
  /* Styles for Landscape Orientation */
  @media (orientation: landscape) {
    body {
      font-size: 25px;
      background-color: rgb(179, 193, 138);
    }
  
    /* Add more styles for landscape orientation as needed */
  }
  </style>
  </head>


  </html>
  <body>
    <h1>Web Application Development</h1>
    <p><a href="http://lms.ai.saveetha.ac.in/">MOODLE FOR AI</a></p>
    <h5>
        Web application development describes the process of designing, building, testing and deploying web-based applications that will be installed on remote servers and delivered to users or customers via the internet.
    </h5>
</body>
</html>
```
## OUTPUT:(iii)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/a79bf020-16ff-4900-91b1-759ffa6778ae)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/223e3063-bf5f-42d6-95b6-0767ec6cc36d)

### Ex-07(iv)-CSS Responsive Typography
## AIM:
To describe how you would use media queries to adjust typography (like font size and line spacing) on a website to improve readability across different device sizes, from mobile phones to large desktop monitors. Include a CSS code snippet in your explanation.

## DESIGN STEPS: 7(iv)
### Step 1:
Identify the HTML elements you want to style. In your case, it’s the div and li elements.

### Step 2:
Define the base styles for these elements. This will be the default styling that applies when no media queries match.

### Step 3:
Use media queries to apply different styles for different device sizes. The @media rule is used in CSS to apply styles for specific media types/devices.

### Step 4:
Inside the media queries, specify the device size for which the styles should apply. You can use min-width and max-width properties to target devices with widths within a certain range.

### Step 5:
Adjust Typography: Inside each media query block, adjust the typography (like font size and line spacing) for the identified elements.

### Step 6:
Test Your Styles.

### Step 7:
Iterate: Adjust your media queries and styles as needed based on your tests.

## CODE: (iv)
```
<!DOCTYPE html>

  <html>
    <head>
    <style>
      body {
        font-size: 16px;
        line-height: 1.5;
      }
     
  @media only screen and (max-width:599px)
   {
    body 
    {
      font-size: 20spx;
      line-height: 1.4;
     /* background-color: cornflowerblue;*/
    }
  }
  
  /* Styles for Medium Screens (Tablets) */
  @media only screen and (min-width: 600px) and (max-width: 1023px)
   {
    body
     {
      font-size: 25px;
      line-height: 1.6;
     /* background-color: rgb(186, 139, 149);*/
    }
  }
  
  /* Styles for Large Screens (Desktop Monitors) */
  @media only screen and (min-width: 1024px) 
  {
    body 
    {
      font-size: 20px;
      line-height: 1.8;
     /* background-color: rgb(140, 209, 186);*/
    }
  }

    </style>
    </head>
  </html>

<html>
<body>
  <h1>Web Application Development</h1>
  <p><a href="http://lms.ai.saveetha.ac.in">MOODLE FOR AI</a></p>
  <h5>
      Web application development describes the process of designing, building, testing and deploying web-based applications that will be installed on remote servers and delivered to users or customers via the internet.
  </h5>
</body>
</html>
```
## OUTPUT:(iv)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/08401858-6b8e-4e0f-a7fd-30683591fa0a)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/649145bb-77a0-4f9d-9bd1-44dbfc96d82e)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/94a38977-b45f-420f-8587-ebe6f5cf83d5)

### Ex-07(v)-Print-friendly CSS
## AIM:
To use a media query to change the styling of a webpage when it is printed, such as changing the background to white and hiding non-essential elements. Provide a CSS example.

## DESIGN STEPS: 7(v)
### Step 1:
Identify the HTML elements you want to style. In your case, it’s the div and li elements.

### Step 2:
Define the base styles for these elements. This will be the default styling that applies when no media queries match.

### Step 3:
Use media queries to apply different styles for different media types. The @media rule is used in CSS to apply styles for specific media types/devices.

### Step 4:
Inside the media queries, specify the media type for which the styles should apply. You can use print to target printers.

### Step 5:
Adjust Styles: Inside each media query block, adjust the styles for the identified elements. You can change the background to white and hide non-essential elements.

### Step 6:
Test your styles using the print preview feature in browsers to ensure they work as expected.

### Step 7:
Iterate: Adjust your media queries and styles as needed based on your tests.

## CODE:(v)
```
<html>
  <head>
    <style type="text/css">
      body {
    background-color: grey;
    color: #333;
  }
  
  .header, .sidebar {
    display: block; /* Keep these elements visible by default */
  }
  
  /* Print Styles */
  @media print {
    body {
      background-color: #fff; /* Change background color to white for printing */
      color: #000; /* Change text color for better readability on print */
    }
  
    .non-esential
     {
      display: none; /* Hide non-essential elements on print */
    }
  
    /* Add more print-friendly styles as needed */
  }

    </style>
  </head>
</html>

<html>
<body>
  <h1>Web Application Development</h1>
  <p><a href="http://lms.ai.saveetha.ac.in">MOODLE FOR AI</a></p>
  <h5>
      Web application development describes the process of designing, building, testing and deploying web-based applications that will be installed on remote servers and delivered to users or customers via the internet.
  </h5>
</body>
</html>
```
## OUTPUT:(v)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/d20a5691-6675-40f8-9f5a-b54b81e79661)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/964ce7fe-db4b-4594-99d8-a96fb86ea651)

### Ex-07(vi)-Dark Mode Implementation
## AIM:
With the increasing popularity of dark mode in user interfaces, explain how you would use a media query to detect if the user has set their system to prefer a dark color scheme. Provide an example of how you would change the background and text colors of a website based on this preference.

## DESIGN STEPS: 7(vi)
### Step 1:
Use the prefers-color-scheme media feature, which is used to detect if the user has requested the system use a light or dark color theme.

### Step 2:
The prefers-color-scheme media feature can have the values light, dark, or no-preference.

### Step 3:
In your CSS, you can use this feature within a @media rule to apply different styles depending on the user’s preference.

### Step 4:
You can set the background color to black and the text color to white when the user prefers a dark color scheme.

### Step 5:
Conversely, you can set the background color to white and the text color to black when the user prefers a light color scheme.

### Step 6:
If the user has no preference, you can choose a default color scheme.

### Step 7:
Remember to test your website in both light and dark modes to ensure the colors work well in both settings.

## CODE: (vi)
```
<!DOCTYPE html>
<html>
<head>
<style type="text/css">
  
    body {
        background-color: white;
        color: black;
    }
    @media (prefers-color-scheme: dark) {
        body {
            background-color: black;
            color: white;
           
            
        }
    }
    @media (prefers-color-scheme: light) {
        body {
            background-color: white;
            color: black;
        }
        
    }
</style>
</head>
<h1>Web Application Development</h1>
  <p><a href="http://lms.ai.saveetha.ac.in">MOODLE FOR AI</a></p>
  <h5>
      Web application development describes the process of designing, building, testing and deploying web-based applications that will be installed on remote servers and delivered to users or customers via the internet.
  </h5>
</body>
</html>
```
## OUTPUT: (vi)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/f85749a3-c8dd-4346-b85b-876170f41954)
![image](https://github.com/anbuselvan1519/ODD2023-WT-Ex-07-CSS/assets/139841744/8ac58a92-f7ff-4038-98b5-3d770ddf391f)

## RESULT:
Therefore the code has been executed successfully.
