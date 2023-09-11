Scripts to help build out a comprehensive svg dataset. 

Function List
| File Name | Description |
| --- | --- |
| md2json.py | Function to loop through each folder and extract the information into a json file |
| getsvg.py | Function to download any svg files in all subfolder html files (from a scraped website) |
| getsvgdata.py | Function to read each svg file and create an array of objects for each svg to include the data. Also writes to csv |
| | |



Shape: 
```
├── brandName ""
├── brandWebsite ""
├── brandPresence[{
│   └── platform
│   └── url
│   └── username}]
├── brandLogo[{
│   └── fileName
│   └── svgPath
│   └── svgData
│   ├── meta
│       │   ├── width
│       │   ├── height
│       │   ├── viewbox
│       │   └── fill
│    └── svgRaw}]
└── brandColors[{
    └── meta
        ├── primary
        ├── secondary
        ├── tertiary
        ├── quaternary
        ├── priority
        └── setting
    ├── colorName
    ├── colorHex
    ├── colorRGB
    ├── colorCMYK
    └── colorPantone}]
```