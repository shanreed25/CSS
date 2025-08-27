# Rows `.rows`
- defines a horizontal group of columns within a container
- rows are essential for grouping columns and ensuring they align correctly within the grid
    - row can be divided into up to 12 equal-width columns
- rows also manage the gutters (spacing) between columns



# Columns `.col`
- represents individual columns within a `row.`
- columns are the building blocks for placing content
- **column size** can be assigned a specific number of the 12 available grid units `col-1` to `col-12`
    - if no specific width is assigned, columns will automatically fill the available space within the row: `col`
- **responsive columns** are breakpoint-specific column classes that control column widths at different screen sizes
    - `col-sm-6`, `col-md-4`, `col-lg-3`
    - enables responsive layouts with a mobile-first approach where styles are defined for smaller screens first and then adjusted for larger ones and content adapts to the viewport
    - For example, `col-md-6` means the column will take 6 out of 12 columns on medium screens and above, while potentially stacking vertically on smaller screens