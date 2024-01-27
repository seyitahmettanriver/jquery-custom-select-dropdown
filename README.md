# Custom Dropdown Plugin

This custom dropdown plugin is a jQuery extension designed with flexibility in mind. You can use it to add a dynamic dropdown menu to your project with a user-friendly interface and various features.

## Features

- **Search Functionality**: Easily filter options in the dropdown menu with the live search feature.
- **Multiple Selection Support**: Allows for selecting multiple options or a single option.
- **Actions Box**: The actions box enables quick actions like selecting all options or clearing selections.
- **Customizable Texts**: Customize the texts displayed in the dropdown menu as you see fit.

## Usage

1. Add the jQuery library to the `<head>` section of your HTML file:

    ```html
    <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
    ```

2. Include the dropdown menu in your project:

    ```html
    <select class="selectpicker" data-count-selected-text="5" data-live-search="true" data-actions-box="true"
            data-text-choose-options="Custom Choose Options"
            data-text-no-results="Custom No Results"
            data-text-deselect-all="Custom Deselect All"
            data-text-select-all="Custom Select All"
            data-text-search="Custom Search..."
            data-text-items-selected="Custom items Selected"
            multiple>
        <option selected>Example</option>
        <option selected>Ketchup</option>
        <option selected>Relish</option>
        <option selected>Mayonnaise</option>
        <option>Hot Sauce</option>
        <option>BBQ Sauce</option>
        <option>Soy Sauce</option>
    </select>
    ```

3. Activate your jQuery plugin on the page:

    ```html
    <script>
        $(document).ready(function () {
            $('.selectpicker').customSelect();
        });
    </script>
    ```

4. You can now use your custom dropdown menu!

## License

This dropdown menu extension is licensed under the [MIT License](LICENSE).
