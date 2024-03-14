# HTML NOTES 

![image](https://github.com/itsme-rash522/frontend-freaks/assets/127365805/b11e5d31-0a9e-4db6-8e37-02fb89d3f213)

## Basic Structure

```html
<!DOCTYPE HTML>
<html>
    <head>
      <title>Title of the document</title>
    </head>
    <body>
      Content goes here
    </body>
</html>
```

## Headings

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

## Paragraphs

```html
<p>This is a paragraph</p>
```

## Line Break

```html
<p>This is the first line.<br>This is the second line.</p>
```

## Horizontal Line

```html
<hr>
```

## Links

```html
<a href="https://www.example.com">Link text</a>
```

## Lists

```html
<!-- Unordered List -->
<ul>
    <li>List item 1</li>
    <li>List item 2</li>
</ul>
<!-- Ordered List -->
<ol>
    <li>List item 1</li>
    <li>List item 2</li>
</ol>
```

## Tables

```html
<table>
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Column 1</td>
      <td>Row 1, Column 2</td>
    </tr>
    <tr>
      <td>Row 2, Column 1</td>
      <td>Row 2, Column 2</td>
    </tr>
  </tbody>
</table>
```

## Forms

```html
<form>
  <lable for="input">Input Label:</lable>
  <input type="text" id="input" name="inputName">

  <lable for="checkbox">Checkbox Label:</lable>
  <input type="checkbox" id="checkbox" name="checkbox" value="checkboxValue">

  <lable>Radio Lable 1:</lable>
  <input type="radio" name="radioName" value="radioValue1">

  <lable>Radio Lable 2:</lable>
  <input type="radio" name="radioName" value="radioValue2">

  <lable for="date">Date:</lable>
  <input type="date" id="date" name="dateName">

  <lable for="number">Number:</lable>
  <input type="number" id="number" name="numberName" min="15" max="100">

  <lable for="color">Color:</lable>
  <input type="color" id="color" name="colorName">

  <lable for="file">File:</lable>
  <input type="file" id="file" name="fileName">

  <button type="reset">Reset</button>
  <button type="submit">Submit</button>
</form>
```

## Images

```html
<img src="image.png" alt="Image description">
```

## Iframes

```html
<!-- Youtube Video -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>

<!-- External Webpage -->
<iframe src="https://www.example.com"></iframe>
```

## Audio

```html
<audio src="audio_file.mp3" controls></audio>
```

## Video

```html
<video src="video_file.mp4" controls></video>
```
