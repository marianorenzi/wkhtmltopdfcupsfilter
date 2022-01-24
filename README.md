# wkhtmltopdfcupsfilter

wkhtmltopdf based CUPS filter to print rendered HTML files

## Supported Attributes
- DefaultPageSize and PageSize
```
*DefaultPageSize: X70MMY65MM
*PageSize X70MMY65MM/80mm x 65mm: "<</PageSize[226 182]>>setpagedevice"
```
- ColorDevice
```
*ColorDevice: False
```

## Supported Options
- Standard PageSize (A4, Legal, Letter, etc. For a full list of supported page sizes please see 
  https://doc.qt.io/archives/qt-4.8/qprinter.html#PaperSize-enum)
- Custom PageSize option
```
lp -o PageSize=Custom.WIDTHxHEIGHT test.html
```