# Key-filters-scripts-
Help filter array of keys as valuesof related key

function getColumn(activeSheet, columnIndex) {
  return activeSheet.getRange(1, columnIndex)
    .getDataRegion(SpreadsheetApp.Dimension.ROWS)
    .getValues()
    .flat();
}

function getRow(activeSheet, rowIndex) {
  return activeSheet.getRange(rowIndex, 1)
    .getDataRegion(SpreadsheetApp.Dimension.COLUMNS)
    .getValues()[0];
}
