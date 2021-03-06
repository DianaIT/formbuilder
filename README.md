# Form Builder with React
![form preview](./public/img/formbuilderpreview.JPG)

## Use
```javascript
import React from "react";
import CustomForm from "./components/CustomForm";
import { LoginForm } from "./Data/loginForm";

export default function App() {
  return <CustomForm props={LoginForm} />
}

```

## Data structure
```javascript
export const LoginForm = {
  title: {
    text: "Form Builder",
    label: "👋🏼",
    labelEmoji: "hello",
  },
  camps: [
    [
      {
        name: "name",
        label: "🙍🏻",
        type: "text",
        placeholder: "John",
      },
      {
        name: "surName",
        label: "🙍🏻",
        type: "text",
        placeholder: "Doe ",
      },
    ],
    [
      {
        name: "checkbox",
        label: "😄",
        type: "checkbox",
        emojiLabel: "happy",
      },

      {
        name: "checkbox2",
        label: "🤣",
        type: "checkbox",
        emojiLabel: "laught",
      },
      {
        name: "checkbox2",
        label: "😇 ",
        type: "checkbox",
        emojiLabel: "saint",
      },
      {
        name: "other",
        label: "👉",
        type: "text",
        emojiLabel: "hand pointed",
        placeholder: "Other",
      },
    ],
    [
      {
        name: "password",
        label: "🔒",
        type: "text",
        emojiLabel: "lock",
        placeholder: "**************",
      },
    ],
    [
      {
        name: "confirmPassword",
        label: "🔒",
        type: "text",
        emojiLabel: "lock",
        placeholder: "**************",
      },
    ],
  ],
  button: {
    text: "GO",
    label: "✒️",
    emojiLabel: "pencil",
  },
};


```