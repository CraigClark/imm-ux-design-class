## Testing and Tools

There are 2 types of testing:

* Accessibility testing against standards
* Usability testing For people with disabilities.

Accessibility testing does not require all the different adaptive technology tools but instead tools for accessibility testing.

Usability testing is best done using the users of those technologies. As an example, you don’t read braille so you cannot effectively test if it would usable by a screen reader user who uses a braille display.

### Tools for accessibility testing

#### Automatic WCAG 2.1 testing

Developer/Accessibility tester cannot rely on automated tools alone when assessing WCAG (Web Content Accessibility Guidelines) 2.1 conformance. Manual testing and human judgement is required on many Success Criteria checks. It’s been found that automated tools give false positive results and make mistakes, also, they can produce misleading results such as not identifying incorrect code.

Web accessibility automated tools alone should not be used to determine conformance levels of Web sites and applications, they can only assist in doing so.

#### Accessibility Testing Tools

Popular automated tools to check accessibility of a website and web application:

* [ComplianceSheriff](https://www.compliancesheriff.com/) can work as a primary layer of batch testing. It will test various standards.

* [Wave](https://wave.webaim.org/) is a free web accessibility tool created by WEBAIM. It is used to validate the web page manually for various aspects of accessibility. This tool can be used to check the intranet, pass-word protected, dynamically generated, or sensitive web pages. Major functions of Web Accessibility Toolbar includes identifying components of a webpage, providing access to alternative view of page content and facilitating the use of third party online applications. It ensures 100% private and secure accessibility reporting
* [aDesigner](http://www.eclipse.org/actf/downloads/tools/aDesigner/) is a tool developed by IBM which simulates the experience of visually impaired individuals so that the designer can better understand the needs of disabled people and develop applications accordingly.
* [aViewer](https://www.tpgi.com/aviewer-2013/) - accessibility API information inspection tool.
* [Vischeck](https://www.betterevaluation.org/en/resources/tool/vischeck) tool is used to simulate how a web page or an image will be viewed by people affected with colour-blindness. This can be done by entering URL or uploading images.
* [Colour Contrast Analyser](https://www.tpgi.com/color-contrast-checker/) is a contast checking tool that can be used outside of web browsers, unlike existing websites and browser addons providing a similar service.
* [WebAIM’s Contrast Checker](https://webaim.org/resources/contrastchecker/) is a browser-based colour contrast analyser.
* [W3C Validator](http://validator.w3.org/) is a code validator and minimum pass requirement to meet [WCAG 2.1 Success Criteria 4.1.1: Parsing](https://www.w3.org/TR/WCAG21/#parsing).
* [Tenon](https://tenon.io/) is a browser-based accessibility checking service.
* [SiteImprove](https://siteimprove.com/en-ca/) is a browser-based accessibility checking service.

#### Web Browsers and add-ons / plug-ins

* [ARIA Validator](https://chrome.google.com/webstore/detail/aria-validator/oigghlanfjgnkcndchmnlnmaojahnjoc?hl=en) for Chrome
* [Web Developer toolbar](https://chrispederick.com/work/web-developer/) for Firefox, Chrome, and Opera
* [Quick Accessibility Page Tester](https://accessify.com/tools-and-wizards/accessibility-tools/favelets/quick-page-test/) is a bookmark that you can click to get a quick analysis of the web page. It will figure out various issues with your page and highlights areas that may benefit to use ARIA.

#### Other automated tools

* **Inspect 32 - Microsoft Windows Object Inspector** is now a feature of [Windows 10 SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/) for embedded web page software or software applications on Microsoft Windows 10 platform.
* [UI Accessibility Checker (AccChecker)](https://docs.microsoft.com/en-us/windows/win32/winauto/ui-accessibility-checker?redirectedfrom=MSDN) verifies that key accessibility requirements are met in the design and implementation of UI Automation (UIA) or Microsoft Active Accessibility (MSAA) regardless of the underlying UI framework.

#### Screen readers

* [Non Visual Desktop Access (NVDA)](https://www.nvaccess.org/) is a free screen-reading software.

**Note:** AAACT recommends user-testing with real users with disabilities instead of purchasing expensive screen reader software for testing. Real users of adaptive technology tend to use the tools differently than testers.

## Other references

* [W3C Web Accessibility Evaluation Tools List](https://www.w3.org/WAI/ER/tools/?q=wcag-20-w3c-web-content-accessibility-guidelines-20)
* [Mozilla: Understanding the Web Content Accessibility Guidelines](https://developer.mozilla.org/en-US/docs/Web/Accessibility/Understanding_WCAG)
* [Canadian Digital Service’s Accessibility Handbook](https://digital.canada.ca/a11y/)
* [Bovernlent of Canada Guide to Planning Inclusive Meetings](https://www.canada.ca/en/employment-social-development/programs/disability/arc/inclusive-meetings.html)

### Accessible documents

* [Accessible Documents Guides | Office 365](https://a11y.canada.ca/en/guides/office365/)
* [PDF accessibility overview](https://www.adobe.com/accessibility/pdf/pdf-accessibility-overview.html)

### WCAG 2.1 requirements

* [How to meet WCAG 2.1](https://www.w3.org/WAI/WCAG21/quickref/?versions=2.1)

* [Understanding WCAG 2.1](https://www.w3.org/WAI/WCAG21/Understanding/)

* [Techniques for WCAG 2.1](https://www.w3.org/WAI/WCAG21/Techniques/)

* [Web Accessibility Tutorials](https://www.w3.org/WAI/tutorials/)

### Mobile accessibility

* [Mobile Optimization - Standard on Optimizing Websites and Applications for Mobile Devices](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=27088)

* [Mobile Accessibility: How WCAG 2.0 and Other W3C/WAI Guidelines Apply to Mobile](https://www.w3.org/TR/mobile-accessibility-mapping/)

* [Google Accessibility](https://www.google.com/accessibility/)

* [Apple Accessibility](https://developer.apple.com/accessibility/ios/)

### Web Experience Toolkit (WET)

WET is an open-source accessible web framework maintained by the Government of Canada. The WET Core serves as an accessible foundation for the [Canada.ca website theme](https://wet-boew.github.io/GCWeb/index-en.html).

* [WET – Working examples](https://wet-boew.github.io/wet-boew/demos/index-en.html)
* [WET – Form validation](https://wet-boew.github.io/v4.0-ci/demos/formvalid/formvalid-en.html)
* [WET – Downloads](https://wet-boew.github.io/v4.0-ci/docs/versions/dwnld-en.html)

Tips for designing and developing Web content:

* [Tips on designing for Web Accessibility](https://www.w3.org/WAI/tips/designing/)

* [Tips on developing for Web Accessibility](https://www.w3.org/WAI/gettingstarted/tips/developing.html)
