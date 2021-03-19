# React-Barcode-Scanner-POC

**DISCLAIMER:  This Proof of Concept asset is being provided as-is to help accelerate your projects.  As such, we are unable to provide official support for this asset.  We have provided documentation as well as any needed code artifacts for your use.**

**Prerequisites:** HCL Commerce V9.1.x / HCL Commerce React Storefront SDK

**It Provide the capability to search HCL Commerce Catalog using barcode recognition on React Stores.**

We have used following components to achieve the voice search

**React Webcam Barcode Scanner** - Capture the barcode from live Image


**Note**

•	The Barcode Scanner currently supports only Code128, EAN and UPC-A. 

•	The library “react-webcam-barcode-scanner “used for scanning barcode does not support the IOS chrome as this library uses HTML5 Media API “getUserMedia” which is not supported by chrome in IOS. Hence, the barcode scan icon would not be displayed for the iOS chrome.

•	Supported Browser are Windows (Chrome, Firefox), Mac (Chrome, Safari, Firefox), Android (Chrome) and iOS(Safari)



**Steps to include the Barcode scanner in your project:**
1. You need to install the react-webcam-barcode-scanner in your project as a dependency.

   `npm install react-webcam-barcode-scanner –save`
   
    Once installation is done. Verify the entry  in your package.json file.
    
2. For icons used,install iconify icons

     `npm install @iconify/react @iconify/icons-mdi`

3. In your Search Bar Widget,import the search-type.tsx and used it as component

    ` import { SearchTypes } from "../Search-types/search-types";`

    `  <SearchTypes showBarcodeIcon={true} setSearchBoxVal={setInput} />`

4. Once All steps are done, Barcode scanner will start working.

  
  
  **Reference**
  
  For more details,refer the ImplementationGuide_BarcodeScanSearch.docx file
 
  

