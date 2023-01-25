# Foundations Courses Conference Demo: HTML and CSS Lesson

## Setting Up Codepen

CodePen is a popular online code editor that allows developers to quickly prototype and share their code. In our courses, Codepen is one of the options teachers can select for students to code in. In order for participants to be able to code, you must create an account and set up a new environment for each "lesson". 

### Step 1: Create an Account

The first step is to create an account on CodePen. Go to https://codepen.io/ and click on the **Sign Up** button in the top right corner. You can sign up using your email address, or by linking your GitHub or Google account.

![Screenshot 2023-01-25 123311](https://user-images.githubusercontent.com/13992684/214684290-a44d837a-70d6-4c2c-afa3-011a3852fffb.png)

Creating an account will allow you to save any work. An account is not required and can by bypassed by clicking **Start Coding** instead.

### Step 2: Create a New Pen

Once you have logged in, you will be taken to your dashboard. To create a new pen, click on the "New Pen" button in the top right corner.

### Step 3: Editor Interface

The editor interface is where you will write your code. It is divided into three main sections:

- **HTML**: This is where you will write the markup for web pages.
- **CSS**: This is where you will write the styling for web pages.
- **JavaScript**: This is where students learn to write code that makes web pages interactive. (Not used in this lesson)

You can switch the layout using the layout button in the editor. 

![Screenshot 2023-01-25 123452](https://user-images.githubusercontent.com/13992684/214684175-08a00d9d-f7b8-4cfa-82db-8dc2b8a352fb.png)

### Step 4: Preview

The preview area is located to the right of the editor. It displays the output of your code. You can switch between the live preview and the debug mode by clicking the button at the top right corner of the preview area.

### Step 5: Save and Share

Once you have finished writing your code, if you've created an account, you can save your pen by clicking the "Save" button in the top right corner. You can also share your pen with others by clicking the "Share" button, which will generate a link that you can send to others.

## Coding Lesson

We will use Codepen to create our very own webpage. To do this we will write code in HTML and CSS. This is a short exercise, so we won't be teaching anything in depth. Follow along with the steps and try to get your webpage up. 

### Step 1: Understanding HTML and CSS

**HTML (Hypertext Markup Language)** is the standard markup language used to create the structure and content of a web page. It is used to create elements such as headings, paragraphs, lists, images, and links on a page.

**CSS (Cascading Style Sheets)** is used to control the layout and presentation of the elements on a web page. It is used to control things like colors, fonts, spacing, and overall layout of a page.

In other words, HTML determines **what exists** is on a webpage, and CSS determines **how it looks**.

#### HTML Syntax

Here is an example of the basic syntax of HTML:

```html
<h1>Welcome to my website!</h1>
<p>This is my first website.</p>
```

In this example, we define the content of the page using **HTML Tags** which tell the page what kind of content is in between them. 

![Screenshot 2023-01-25 124951](https://user-images.githubusercontent.com/13992684/214687462-cb89d01e-012f-4e3c-8651-c07de7c11cfd.png)

- `<h1></h1>`: Describes a heading of level 1 (the largest)

- `<p></p>`: Describes a paragraph.

Note that the second tags always have a slash `/` this tells the page that it is done describing the content. 

#### CSS Syntax
Here is an example of the basic syntax of CSS

![image](https://user-images.githubusercontent.com/13992684/214689522-e0556e32-7f06-41bc-92f9-731473ab046e.png)

- `selector`: Selects the html elements we want to set the appearance of.
- `property`: The aspect of the element we want to set. 
- `value`: What we are setting the property to. 

Let's say we want to make our HTML heading from earlier red and larger. We have to select `h1`, and set the `color` property to the value `red`. Then in the same block we can set the `font-size` property to `20px`. 

```css
h1 {
 color: red;
 font-size: 20px;
}
```

### Step 2: Getting Started

Start the project from a clean slate. The first thing we're going to do is add a heading to our page. You can title your page anything you want.

#### HTML

```html
<h1>My First Webpage</h1>
```

We creating a heading by writing our own title text in between opening `<h1>` and closing `</h1>` tags.

![Example of heading with only html](https://user-images.githubusercontent.com/13992684/214693288-0e9da244-c150-4a35-b398-8f05fa71c1fd.png)


Then we can use CSS to change how it looks.

#### CSS

```css
h1 {
 font-family: sans-serif;
 text-align: center;
}
```

![Example of heading with html with css](https://user-images.githubusercontent.com/13992684/214693179-f57410e4-15fc-4c41-827a-4302660f4a48.png)

In your page, you can choose different values. Here are some you can try out:

For `font-family` choose from:
- `serif` 
- `sans-serif` 
- `monospace` 
- `cursive` 
- `fantasy` 
- `Arial` 
- `Helvetica`
- `Times`

For `text-align` choose from:
- `center`
- `left`
- `right`

### Step 3: A Splash of Color

#### Find a Background Color

Colors in CSS are represented in many ways. The easiest way to describe a color is using a color picker. Google has a color picker built in if you search "color picker". 

![Google color picker](https://user-images.githubusercontent.com/13992684/214694805-5f8aa2bd-4170-4006-ac59-8c78cdef35f9.png)

We are going to select a background for our page, use the color picker to find a color you like and copy the hex code e.g. `#ffcd17`. Now we can use it in our CSS to change the background of our website. 

To access the background, we can use the `body` selector and set its `background-color` to the color you picked.

#### CSS

```css
body {
  background-color: #f2b611;
}

h1 {
 font-family: sans-serif;
 text-align: center;
}
```

![Changing the background color](https://user-images.githubusercontent.com/13992684/214695218-9ac0efce-16d0-45c1-807c-652d940ac182.png)

### Step 4: Make Your Heading Pop!

When you write text, it's important to have a high contrast with the background so its easy to read. Since our text is black, we can make the heading pop by giving it a white background and making it look like its in a banner. We can do this by setting four properties. Try adding them one at a time and see what they do.

#### CSS

```css
body {
  background-color: #f2b611;
}

h1 {
 font-family: sans-serif;
 text-align: center;
  
 background-color: white;
 padding: 16px;
 margin: 16px;
 border-radius: 8px;
}
```

![Heading styled as a banner](https://user-images.githubusercontent.com/13992684/214696409-5868a994-cd7d-4bfc-afc9-af1a27c85248.png)

### Step 5: Adding Media

A site with only text can be a little boring. By adding media like images we can add variety and engagement to the page. Find an image on the web and copy the link to the url. Try to find an image that fits in with the background color you chose.

Be sure that you don't just copy the link to the website. To do this, find the image you want to use and click "Copy Image Address".

![image](https://user-images.githubusercontent.com/13992684/214703551-eac52121-aeec-4604-9c87-7f26816addb3.png)

Once you have it in your clipboard, you can paste it into the `src` attribute of an `img` tag in your html.

#### HTML

```html
<h1>My First Webpage</h1>
<img src="https://paste-your-image-link-here.jpg" />
```

Your image may be way too large for the page or much too small. But we can fix that by adding this block to your CSS.

#### CSS

```css
img {
  width: 300px;
  height: 300px;
  
  display: block;
  margin: auto;
  
  padding: 16px;
  background-color: white;
}
```

The CSS above does three things.
1. Use `width` and `height` properties to set the size of the image. (Feel free to tweak these numbers and see what happens).
2. Use `display: block;` and `margin: auto` to center the image on the page. (This is covered in greater detail in the full course).
3. Use `padding` and `background-color` properties to add a frame to the image.

#### Result

![image](https://user-images.githubusercontent.com/13992684/214705856-62306c8d-0408-4869-8582-13f7ca77e4cd.png)

### Review

In only a few minutes, you've used two coding languages to create your first webpage. Here is an example of what your final code could look like.

#### HTML

```html
<h1>My First Webpage</h1>
<img src="https://user-images.githubusercontent.com/13992684/214703816-71331bdc-ca1f-4723-a66d-c2219dc27928.png" />
```

#### CSS

```css
body {
  background-color: #E3A81D;
}
h1 {
 font-family: sans-serif;
 text-align: center;
  
 background-color: white;
 padding: 16px;
 margin: 16px;
 border-radius: 8px;
}
img {
  width: 300px;
  height: 300px;
  
  display: block;
  margin: auto;
  
  padding: 16px;
  background-color: white;
}
```







