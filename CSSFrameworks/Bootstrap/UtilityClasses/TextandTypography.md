## Font Sizes
- responsive font size utility classes range from `.fs-1` (largest) to `.fs-6` (smallest)
- can be directly applied to any HTML element to quickly adjust its font size
- The best method depends on your specific needs
    - utility classes for quick adjustments
    - Sass for comprehensive customization
    - custom CSS for specific overrides

### Sass Customization
- for more granular control and consistent styling across your project, you can customize Bootstrap's Sass variables
- `$font-sizes` Sass map allows you to define custom font sizes for the utility classes
- `$font-size-base` controls the default base font size for the entire application.
```
    // Example of customizing font sizes in a Sass file
    $font-sizes: (
      1: 5rem,
      2: 4rem,
      3: 3rem,
      4: 2rem,
      5: 1.5rem,
      6: 1rem
    );

    // Set a custom base font size
    $font-size-base: 18px; 
```

### Custom CSS
- override Bootstrap's styles by writing your own custom CSS rules
- provides the most flexibility but can lead to more complex stylesheets if not managed carefully