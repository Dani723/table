# [VCL](https://github.com/vcl/doc) table

Display tabular data.

## Features

The following basic aspects of table formatting are
covered by the offered table variants:

_Cell and column highlighting_

Single cells and columns can be highlighted by using the `vclCellHighlight`
class on each `td`in the respective column or on single cells only.
An example is shown in the fourth column.

_Column width_

The column width can be defined in the table header using one of the classes `vclSpan-5p` - `vclSpan-90p`.
which define the occupied space in percent.

_Heading height (two lines of text)_

The class `vclDblHead` is used for two-line-table-headings in order to vertically align the button in the middle.
Additionally the text and the button have to be wrapped inside a `div` respectively. Please see the code of the Multi-selection Table as an example.

_Column sortability_

Sortable columns are defined with the `vclSortableCol` class on the respective `th`s.
This class gives the whole header a pointer cursor to indicate its sortability.
The application must register an appropriate event handler to change the sort order for the whole `th` accordingly.
Also an icon which indicates sortability should be used as shown in the second column.
The currently active sort order is indicated by a respective icon and the classes `vclSortAsc`
or `vclSortDesc` on the `th` as shown in the third column.
If a column is sorted, all columns of the table must be sorted according to this order.

_Row selectability_

Rows can be configured to be selectable (check or radio style).
If rows are selectable, the `tbody` has the class `vclRowSelectability` and
a selected row has the class `vclSelected`.

If a table spans more than one page, every `tr` must be given the attribute `data-index`
with a sequential number. The table selection logic uses this index in conjunction with a user-supplied hidden form field
to keep track of the selections.

_Row hovering_

If a table row should be highlighted on hover, the `vclRowHoverHighlight` modifier can be used.

_Row action_

Actions applicable to a row as shown in the last column of the example below
can be realized using links or any form interaction element like a button.

_Global action_

Actions applicable to the whole table or the set of selected rows can be realized
with a tool bar by using the class `vclTableToolbar` as shown in the sum table exmple.

_Alternating row color_

Optionally an alternating row color can be defined by using the class `vclAltRowColor` for the `table` element.

_Border configuration_

No border is shown with `vclNoBorder`.
The border style can be changed from solid to dotted by using the `vclDottedBorder` modifer.

_Padding style_

If the default cell padding is too extensive, `vclCondensed` makes it more compact as shown in the
multi selection example.

_Text alignment_

Left alignment is default, for centered text use class `vclAlignCentered` and for right aligned text
`vclAlignRight` on `td`s.

_Vertical alignment_

Top alignment is default, for vertically centered content use class `vclVAlignMiddle` and for bottom aligned content
`vclVAlignBottom` on a `table` or `td`s.

_Pagination_

The pagination control can optionally be combined with any table.

_Layout_

The `auto` layout mode is used by default. For tables with toolbars however,
the `vclFixed` class must be used.

_Truncation_

In conjunction with the fixed layout mode, the modifier `vclSingleLine` can be used to truncate cell content which would span more than one line and show an ellipsis to indicate truncated content instead.

_Wrapping aehavior_

To allow breaking words of textual cell content apart, use the modifier `vclBreakWords`. This works best in combination with the fixed layout mode.

## Usage

## Classes

- `vclTable`

## Modifiers

- `vclCellHighlight`
- `vclDblHead`
- `vclSortableCol`
- `vclSortAsc`
- `vclSortDesc`
- `vclRowSelectability`
- `vclSelected`
- `vclRowHoverHighlight`
- `vclAltRowColor`
- `vclNoBorder`
- `vclCondensed`
- `vclAlignCentered`
- `vclAlignRight`
- `vclVAlignMiddle`
- `vclVAlignBottom`
- `vclSingleLine`

## Variables

- `--table-color`
- `--table-disabled-color`
- `--table-border-color`
- `--table-bg-color`
- `--table-header-bg-color`
- `--table-header-color`
- `--table-header-button-hover-color`
- `--table-footer-bg-color`
- `--table-footer-color`
- `--table-alt-bg-color`
- `--table-highlight-bg-color`
- `--table-highlight-hover-bg-color`
- `--table-row-selected-color`
- `--table-row-selected-bg-color`

## Demo

[example.html](/demo/example.html) on GH-pages.
