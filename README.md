# Welcome to Strawberry UI

Welcome to the Strawberry UI repository, a vibrant and visually stunning UI library inspired by the sweet and juicy fruit - the strawberry.

Our goal with Strawberry UI is to incorporate the playful and energetic colors of a strawberry into its layout and design, creating a lively and engaging user interface. This library is made possible by the collaboration between Midjourney and ChatGPT platforms, leveraging the expertise of both products to create a unique and exciting UI experience.

One of the unique features of Strawberry UI is its integration with ChatGPT, which exposes prompts to guide users through the UI design process. This means that you can easily create beautiful and functional interfaces with the help of a powerful AI assistant.

Whether you are a designer, developer, or just someone who loves to create beautiful things, Strawberry UI has something to offer. With its intuitive and easy-to-use components, you can quickly build stunning UIs that are both visually appealing and highly functional.

We hope that you enjoy using Strawberry UI as much as we enjoyed creating it. If you have any feedback or suggestions, please feel free to reach out to us. Happy designing!

## Components API

### Music Widget
MusicWidget Component README File

The MusicWidget component is a styled component that displays a music player interface. The widget has a width of 350px and a height of 405px. It has the following subcomponents:

| Subcomponent         | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Wrapper              | The main container for the MusicWidget component.                            |
| TopSection           | A container for the top section of the MusicWidget component.                |
| TopSectionBg         | A container for the background of the top section.                           |
| TopSectionBorder     | A container for the border of the top section.                               |
| TitleAlbumWrapper    | A container for the title and album information.                             |
| Title                | A styled component for the title of the song.                                 |
| Author               | A styled component for the author of the song.                                |
| Album                | A styled component for the album name.                                       |
| SvgPlayButton        | A SVG component for the play button.                                         |
| Button               | A button component for controlling the music.                                |
| Rectangle            | A subcomponent of the Button component.                                      |
| PlayIcon             | A SVG component for the play icon.                                           |
| NextIcon             | A SVG component for the next icon.                                           |
| PrevIcon             | A SVG component for the previous icon.                                       |

The MusicWidget component requires the following props:

| Prop         | Type     | Description                                               |
|--------------|----------|-----------------------------------------------------------|
| theme        | string   | The theme of the widget (either 'dark' or 'light').         |
| title        | string   | The title of the song.                                     |
| author       | string   | The author of the song.                                    |
| album        | string   | The album name.                                            |
| onPlay       | function | A function to be called when the play button is clicked.   |
| onNext       | function | A function to be called when the next button is clicked.   |
| onPrevious   | function | A function to be called when the previous button is clicked.|


The MusicWidget component uses the styled-components library for styling. The PropTypes library is also used to define the prop types for the component.

### Login Page
**LoginPage Component Documentation**

`LoginPage` is a styled React component that provides a login form with two input fields (username and password), a submit button and a background image. It uses `TextField` component for the input fields.

The component has the following structure:

```
<LoginPage
  theme="light" // the color theme of the component ("light" or "dark")
  width={400} // the width of the component in pixels
  onSubmit={handleSubmit} // the callback function that is called when the form is submitted
/>
```

The component has the following subcomponents:

- `Wrapper`: the outermost container of the component that holds the background and the form.
- `WrapperBackground`: a transparent layer that covers the background image of the component.
- `WrapperBorder`: a gradient layer that covers the border of the component.
- `Container`: a container that holds the form and the background image.
- `ContainerBg`: a container that holds the background image.
- `ContainerBorder`: a gradient layer that covers the border of the form.
- `Header`: a container that holds the title of the component.
- `LoginText`: the title of the component.
- `Form`: the form that holds the input fields and the submit button.
- `Row`: a container that holds an input field and its icon.
- `LoginButtonWrapper`: the submit button.

The component can be styled using the following props:

- `theme`: the color theme of the component ("light" or "dark"). The default value is "light".
- `width`: the width of the component in pixels. The default value is 400 pixels.
- `onSubmit`: the callback function that is called when the form is submitted. The default value is an empty function.

### Time Widget
## TimeWidget Component

The `TimeWidget` component is a React component that displays a list of times in three separate columns that can be scrolled independently. The user can select a time by clicking on it, and the selected time will be highlighted in the center column. The component also includes a title and a selected time display.

### Usage

To use the `TimeWidget` component, simply import it and use it like any other React component:

```javascript
import { TimeWidget } from "./TimeWidget";

function MyApp() {
  return (
    <div>
      <TimeWidget />
    </div>
  );
}
```

### Props

The `TimeWidget` component does not accept any props.

### Styling

The `TimeWidget` component is styled using CSS-in-JS with styled-components. The following styled-components are exposed for customization:

- `Container`: styles the outermost container of the component.
- `TitleContainer`: styles the container for the component title.
- `Title`: styles the component title.
- `ListContainer`: styles the container for the time list.
- `List`: styles the individual columns of the time list.
- `ListItem`: styles the individual items in the time list.
- `EmptyItem`: styles the empty item in the center of the time list.
- `SelectedContainer`: styles the container for the selected time display.
- `SelectedColumn`: styles the individual columns in the selected time display.

### To Do List
## To Do List Component

This is a To Do List component built with React and styled-components, which allows users to add, edit and remove items from a list. The component has a customizable background and strawberry decorations.

### Usage

1. Import the component:

```javascript
import ToDoList from './ToDoList';
```

2. Render the component:

```javascript
<ToDoList />
```

### Props

The component accepts the following props:

| Prop      | Type     | Default | Description                                             |
| --------- | -------- | ------- | ------------------------------------------------------- |
| `theme`   | `string` | `'light'` | Theme for the component (`'light'` or `'dark'`)          |

### Dependencies

This component depends on the following packages:

- `React` (v16.8.0 or higher)
- `styled-components` (v5.0.0 or higher)
- `TextField` component
- `PrimaryButton` component

### Example

```javascript
import React from 'react';
import ToDoList from './ToDoList';

function App() {
  return (
    <div>
      <ToDoList theme="light" />
    </div>
  );
}

export default App;
```

### Calendar
# Calendar Component

This is a React component that displays a calendar for a given month. The component has several customizable features such as theme, selected date and onDateChange function.

## Usage
To use the Calendar component, you will need to import it into your React application and render it using the following syntax:

```jsx
import Calendar from './path/to/Calendar';

function App() {
  return (
    <div>
      <Calendar />
    </div>
  );
}

export default App;
```

### Props

The Calendar component accepts the following props:

| Prop             | Type        | Default Value | Description                                                                                                                                                                                                                                                                                                                        |
|------------------|-------------|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `selectedDate`     | `Date`      | `new Date()`     | The selected date to highlight in the calendar.                                                                                                                                                                                                                                                                                   |
| `onDateChange`     | `function`  | `() => {}`       | The function to be called when the user selects a date in the calendar. It will be passed the selected date as an argument.                                                                                                                                                                                                       |
| `theme`            | `string`    | `dark`          | The theme to use for the calendar. Possible values are `'dark'` and `'light'`.                                                                                                                                                                                                                                                    |

### Styling

The Calendar component can be styled using CSS. The following CSS selectors can be used to target specific elements:

| Selector           | Description                                                                                                                                                                                                                                                                                                                                                                                          |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `.WidgetContainer`  | The main container that wraps the entire calendar.                                                                                                                                                                                                                                                                                                                                                   |
| `.Header`           | The container that wraps the month and year display and the previous and next buttons.                                                                                                                                                                                                                                                                                                            |
| `.MonthYear`        | The container that displays the current month and year.                                                                                                                                                                                                                                                                                                                                               |
| `.DaysOfWeek`       | The container that displays the days of the week.                                                                                                                                                                                                                                                                                                                                                    |
| `.DayOfMonth`       | The container that displays each day of the month.                                                                                                                                                                                                                                                                                                                                                    |
| `.active`           | The class added to the container that displays the currently selected date.                                                                                                                                                                                                                                                                                                                         |
| `.StyledWeekContainer` | The container that wraps each week of the calendar.                                                                                                                                                                                                                                                                                                                                                   |
| `.DecoratingLine`   | The line that separates the month and year display from the calendar grid.                                                                                                                                                                                                                                                                                                                           |
| `.StyledDaysOfWeek` | The container that displays each day of the week in the calendar grid.                                                                                                                                                                                                                                                                                                                               |
| `.DecoratedWonkyStrawberryBg` | The background image of the calendar.                                                                                                                                                                                                                                                                                                                                                                 |
| `.StyledButtonsWrapper` | The container that wraps the previous and next buttons.                                                                                                                                                                                                                                                                                                                                               |

## Example
Here's an example of how to use the Calendar component with all props set to their default values:

```jsx
import Calendar from './path/to/Calendar';

function App() {
  return (
    <div>
      <Calendar />
    </div>
  );
}

export default App;
```

### Slider
Here is a short documentation for the Slider component:

## Slider Component

The Slider component is a custom slider created with React and styled-components. It has a strawberry-shaped handle and two lines on each side to indicate the value range. The slider can be used to select a value within a range.

### Props

- `theme` (optional): determines the color scheme of the slider. Possible values are `'dark'` (default) and `'light'`.

### Example Usage

```jsx
import Slider from './Slider';

function App() {
  return (
    <div>
      <Slider theme="dark" />
      <Slider theme="light" />
    </div>
  );
}
```

### Pagination
# Pagination Component Readme

The Pagination Component is a React component that can be used to render a pagination bar with clickable buttons for navigating through a list of pages. 

## Usage

The component can be imported and used in a React application like any other React component. 

```
import Pagination from './components/Pagination';

function App() {
  const totalElements = 100;
  const elementsPerPage = 10;

  const handlePageChange = (pageIndex) => {
    console.log(`Navigating to page ${pageIndex}`);
  }

  return (
    <Pagination 
      totalElements={totalElements} 
      elementsPerPage={elementsPerPage} 
      onPageChange={handlePageChange} 
    />
  );
}
```

## Props

The Pagination Component accepts the following props:

| Prop Name       | Type     | Required | Default Value | Description                                                                                                                                                                                                                                                                                                                                                                                               |
| ---------------| -------- | -------- | -------------| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| totalElements   | number   | Yes      | N/A          | The total number of elements to paginate.                                                                                                                                                                                                                                                                                                                                                                 |
| elementsPerPage | number   | Yes      | N/A          | The number of elements to display per page.                                                                                                                                                                                                                                                                                                                                                                |
| onPageChange    | function | Yes      | N/A          | A callback function that is invoked when a page button is clicked. The function is called with the index of the page that was clicked.                                                                                                                                                                                                                                                                      |
| theme           | string   | No       | 'dark'       | The color scheme of the pagination bar. Possible values are 'dark' and 'light'.                                                                                                                                                                                                                                                                                                                            |

## Styling

The Pagination Component uses styled-components for styling. The following styled components are used:

| Component Name                     | Description                                                                                                                                                                                |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `PaginationContainer`              | The container element for the entire pagination bar.                                                                                                                                        |
| `PageNumber`                       | The button element for each individual page number.                                                                                                                                         |
| `ArrowButtonLeft`                  | The button element for the left arrow.                                                                                                                                                      |
| `ArrowButtonRight`                 | The button element for the right arrow.                                                                                                                                                     |
| `StyledPagesContainer`             | The container element for the page number buttons.                                                                                                                                          |
| `StyledLeftGreenDecorationWrapper` | A styled wrapper for the green decoration on the left side of the pagination bar.                                                                                                          |
| `StyledRightGreenDecorationWrapper`| A styled wrapper for the green decoration on the right side of the pagination bar.                                                                                                         |

Each styled component has its own set of CSS rules that can be customized by passing props to the component. For example, to change the background color of the pagination bar, you can pass a `theme` prop with the value 'light':

```
<Pagination totalElements={100} elementsPerPage={10} onPageChange={handlePageChange} theme='light' />
```

### TextField
## TextField Component

The `TextField` component is a reusable input field component that can be used in a variety of React applications. It has the following features:

- Accepts an `onSubmit` function to handle form submission
- Accepts an `onChange` function to handle input changes
- Accepts a `placeholder` string to display a placeholder text in the input field
- Accepts a `controlledValue` prop to control the value of the input field from the parent component
- Can be set as a password field by setting the `isPassword` prop to `true`
- Can be set to use a light or dark theme by setting the `theme` prop to either `'dark'` or `'light'`

### Usage

To use the `TextField` component in your React application, simply import it and use it like any other React component. Here's an example:

```javascript
import React, { useState } from 'react';
import TextField from './TextField';

const MyForm = () => {
  const [inputValue, setInputValue] = useState('');

  const handleSubmit = (value) => {
    console.log('Submitted value:', value);
  };

  const handleChange = (value) => {
    setInputValue(value);
  };

  return (
    <form onSubmit={(e) => e.preventDefault()}>
      <TextField
        onSubmit={handleSubmit}
        onChange={handleChange}
        placeholder="Enter your name"
        controlledValue={inputValue}
        theme="light"
      />
    </form>
  );
};
```

### Props

The `TextField` component accepts the following props:

| Prop name        | Type     | Default value             | Description                                                                                                                                                                                                                                                                                                             |
| ---------------- | -------- | ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `onSubmit`       | Function | `undefined`               | A function to handle form submission. The function will be called with the current value of the input field as its argument.                                                                                                                                                                                            |
| `onChange`       | Function | `undefined`               | A function to handle input changes. The function will be called with the current value of the input field as its argument. If the `controlledValue` prop is provided, the input field will be controlled by the parent component and this function will not be called.                                                    |
| `placeholder`    | String   | `'Strawberry Fields Forever'` | The placeholder text to display in the input field.                                                                                                                                                                                                                                                                      |
| `controlledValue`| String   | `undefined`               | The value to control the input field from the parent component. If this prop is provided, the input field will be controlled by the parent component and the `onChange` function will not be called.                                                                                                                     |
| `isPassword`     | Boolean  | `false`                   | Whether the input field should be displayed as a password field. If `true`, the input will hide the entered text with `*` or bullet points.                                                                                                                                                                             |
| `theme`          | String   | `'dark'`                  | The theme of the input field. Can be set to either `'dark'` or `'light'`.                                                                                                                                                                                                                                                |