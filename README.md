# Custom Bootstrap Subtheme

This is a subtheme for Drupal based on the contributed Bootstrap theme. It provides custom styles and theme functions to enhance the appearance and functionality of your Drupal website.

## Theme Features

- Light blue color scheme.
- Custom styles for blocks and the login page.
- Custom theme function for rendering the menu tree.

## Usage

1. **Installation:**
   - Download and enable the Bootstrap base theme (if not already installed).
   - Clone or download this subtheme into the `themes` directory of your Drupal installation.

2. **Configuration:**
   - Set the subtheme as the default theme in Drupal's administration interface.

3. **Customization:**
   - Adjust the Sass files (`custom-bootstrap-subtheme.scss`, `blocks.scss`, `login.scss`) to match your design preferences.
   - Customize the menu rendering in `custom-bootstrap-subtheme.theme` as needed.

## Menu Theme Function

The following sample shows a subtheme based on the contributed Drupal Bootstrap theme. The subtheme provides a custom theme function for rendering the menu tree.

```php
// custom-bootstrap-subtheme.theme

/**
 * Theme function for rendering a menu with Bootstrap dropdowns.
 */
function custom_bootstrap_subtheme_menu_tree($variables) {
  return '<ul class="nav">' . $variables['tree'] . '</ul>';
}
