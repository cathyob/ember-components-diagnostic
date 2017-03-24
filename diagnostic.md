# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    Shopping List - a shopping list is made of items
     |_ Items - items belong to a list
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember generate componenet my-map
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    components > .js - houses any actions, class names/bindings, etc.
    templates > components > .hbs - houses the template portion
    tests > integration > components > .js
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
    {{contact/my-contact my-contact=my-contact}}
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-contact.my-phone}}
    ```
