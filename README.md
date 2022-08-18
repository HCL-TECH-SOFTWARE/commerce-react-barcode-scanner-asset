# React-Barcode-Scanner-Asset

## WARRANTY & SUPPORT 
HCL Software provides HCL Commerce open source assets “as-is” without obligation to support them nor warranties or any kind, either express or implied, including the warranty of title, non-infringement or non-interference, and the implied warranties and conditions of merchantability and fitness for a particular purpose. HCL Commerce open source assets are not covered under the HCL Commerce master license nor Support contracts.

If you have questions or encounter problems with an HCL Commerce open source asset, please open an issue in the asset's GitHub repository. For more information about [GitHub issues](https://docs.github.com/en/issues), including creating an issue, please refer to [GitHub Docs](https://docs.github.com/en). The HCL Commerce Innovation Factory Team, who develops HCL Commerce open source assets, monitors GitHub issues and will do their best to address them. 

## HCLC Barcode Scanner Integration Asset

**Prerequisites:** HCL Commerce V9.1.x / HCL Commerce React Storefront SDK

**It Provide the capability to search HCL Commerce Catalog using barcode recognition on React Stores.**

We have used following components to achieve the Barcode scanner

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

**Update Aug-2022**
• react-webcam-barcode-scanner has been deprecated earlier year. Customers using this asset should use react-qr-barcode-scanner library.

• Supported Browser details given at https://www.npmjs.com/package/react-qr-barcode-scanner
  
  **Reference**
  
  For more details,refer the ImplementationGuide_BarcodeScanSearch.docx file
 
  

