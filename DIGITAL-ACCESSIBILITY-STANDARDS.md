# Digital Accessibility Standards VisitScotland

- [Digital Accessibility Standards VisitScotland](#digital-accessibility-standards-visitscotland)
  - [Introduction](#introduction)
  - [Text and Typography](#text-and-typography)
  - [Colour and Contrast](#colour-and-contrast)
  - [Multimedia](#multimedia)
      - [Pre-recorded audio only](#pre-recorded-audio-only)
      - [Pre-recorded video only](#pre-recorded-video-only)
      - [Use of Decorative Images](#use-of-decorative-images)
  - [Accessibility Testing](#accessibility-testing)
    - [Manual Testing](#manual-testing)
    - [Automated Testing](#automated-testing)
    - [Assistive Technologies](#assistive-technologies)
    - [Testing Principles](#testing-principles)

## Introduction

This document is an extension to VisitScotland’s Digital Partners Standards Document.

As a Public Sector Organisation, VisitScotland has a [legal obligation to make sure digital information can be accessed by everyone](https://www.gov.uk/guidance/accessibility-requirements-for-public-sector-websites-and-apps). It is the belief of the Organisation that no-one should be excluded because of a disability. Users must feel included and valued to be engaged, therefore VisitScotland strives to make digital products universally accessible and useful. VisitScotland is inclusive as an organisation. 

To meet VisitScotland’s accessibility requirements, digital assets or products must:
- meet level AA of the Web Content Accessibility Guidelines (WCAG 2.2) as a minimum.
- function correctly on the most common assistive technologies - including screen magnifiers, screen readers and speech recognition tools.

On average, up to 57% of WCAG issues can be identified automatically. Reliable automation testing tools such as Deque Axe and auditing tools such as Google Lighthouse, include prompts for additional items to checked manually. 

To ensure digital assets or products meet all AA requirements, evidence must be provided to show:
- manual testing has been carried out in addition to any automation testing.
- the asset or product was tested with assistive technology.

It is recommended manual testing should include end-to-end testing using assistive technology such as screen readers to fully consider the accessible user experience. 
Acceptable evidence includes a spreadsheet recording test results, automated script logs or assistive technology recordings.

For more detail on accessibility recommendations, visit the WCAG website at: [WCAG2.2](https://www.w3.org/TR/WCAG22/)

## Text and Typography

There are several considerations that must be made in the application of text to ensure that content is accessible. These include: 
- Using sans-serif fonts (for example, Roboto, Helvetica or Arial instead of Georgia for body text) 
- Using fonts that are compatible with screen readers 
- Ensuring default text size of 14px 
- Using optimum line length and character count
- Ensuring adequate character and line spacing
- Ensuring adequate contrast 
- Avoiding hyphenation of text 
- Avoiding justification of text


## Colour and Contrast 

To provide good contrast, the contrast ratio between the text and background should be greater than or equal to 4.5:1 for small text and 3:1 for large text.

[WCAG Guideline 1.4.3 Level AA Contrast](https://www.w3.org/WAI/WCAG22/quickref/?versions=2.2#contrast-minimum)

**Note:** Font choices, sizes and the cut off between what is deemed large text and small text should be agreed with VisitScotland at the outset.

__Exceptions:__

- Colour contrast ratio requirements apply to text and graphics that are essential for understanding the content or functionality. The above colour contrast requirements do not apply for logos or incidental graphic elements. 
- Text that is part of a logo has no minimum contrast requirement.  
- Text that is part of disabled control states or disabled buttons do not need to meet the minimum contrast ratio. 

The contrast between the text and background colour should be slightly tempered. For example: Pure black text on a pure white background should not be used. Stark contrast can result in blurred or moving text for people with Irlen syndrome. 

When using text over images a solid background behind the text or a dark overlay to the image should be added.
Several contrast checkers are available online for comparing how accessible background and text colour combinations are. One such WCAG compliant checker is available at [contrastchecker.com](https://contrastchecker.com/).


## Multimedia

### Pre-recorded audio only: 

An alternative for time-based media should be provided to present equivalent information for pre-recorded audio-only content. 

### Pre-recorded video only:

Either an alternative for time-based media or an audio track should be provided to present equivalent information for pre-recorded video-only content. Audio descriptions should be provided for all pre-recorded video content in synchronized media to meet AA standard.

- A modern video player that supports captions should be used.
- Captions should be synchronized to appear around the same time that they would be heard in the audio. 
- Captions do not need to be a word-for-word version of the audio but should be a concise equivalent. 
- Transcripts should be provided as one of the optional output formats produced by the closed captioning process. 
- In making the transcript available, link to it from the web page, wherever linking to or displaying the associated video. 

See the separate ‘VisitScotland Accessible Video & Audio Guidelines’ document for further details.

Digital Partners can find further information on media accessibility with [WCAG Guideline 1.2 – Time-based Media](https://www.w3.org/WAI/WCAG22/quickref/?versions=2.1#audio-only-and-video-only-prerecorded) and accessible design from the [UK Government – Do’s and Don’ts on Designing for Accessibility](https://accessibility.blog.gov.uk/2016/09/02/dos-and-donts-on-designing-for-accessibility/).

### Use of Decorative Images

The nature of VisitScotland’s digital estate requires the use of images that end users will find inspirational. However, the announcement of these images to a screen reader user can be overwhelming and repeatedly attributes to ‘audible clutter’. As such, any images which do not add information to the content of the page are considered as Decorative Images.

These images require the addition of an empty or null alt text attribute in the HTML code as this will instruct the screen reader to skip over them. A null alt text is written as **alt=""**. Not providing an empty alt text attribute will result in some screen readers announcing the name of the image file instead. 

Functional and informative images may also be required for a VisitScotland digital asset. In these cases, it should be considered if the information provided by the image is useful or required by the user, and if so, this information should be provided appropriately.

Further information on image classification and best practice can be found on the [W3C images tutorial](https://www.w3.org/WAI/tutorials/images/).

## Accessibility Testing 

Human interaction is the most reliable method to assess accessibility. Therefore, automated testing needs to be combined with ongoing manual testing to ensure that true accessibility is being achieved.

### Manual Testing 

Manual testing should be a combination of:
- following an accessibility test list or set of test-cases.
- simulate real user experience with end-to-end testing.

Carried out alongside automated testing, manual accessibility testing should focus on aspects of; error identification, focus order and keyboard support on custom controls, and screen reader testing. 

Many accessibility auditing tools such as Google Lighthouse and Deque Axe will provide details on additional manual testing which has not been captured by the automation. 

The [18F accessibility guide](https://guides.18f.org/accessibility/) provides a checklist and simple test procedures to test common accessibility aspects of digital applications and it is recommended that Digital Partners utilise these in their testing procedures.

**Digital Partners are required to provide VisitScotland with a Test Summary document to show a manual accessibility test has been carried out. This should include details of; operating System, device, browser version, project, task, result, name of tester, date, and details of any errors.**

### Automated Testing 

When carried out alongside manual accessibility testing, automated testing should focus on:
- HTML hierarchy and relationships.
- correct use of ARIA or screen reader roles.
- colour contrast.
- form controls.
- links and buttons have accessible names.

VisitScotland recommends using a combination of accessibility auditing and linting tools to check for common accessibility errors. 
Recommended tools include:
- Deque Axe tools
- Google Lighthouse
- WebAIM WAVE Extension
- Microsoft Accessibility Insights.io
- SiteImprove
- SortSite
- Deque Axe Accessibility Linter
- ESLint Accessibility Plugin

It is recommended that accessibility linting tools and other test automation is integrated into the Software Development Lifecycle to catch errors as digital assets are designed, developed, and built.

**Digital Partners are required to provide VisitScotland with a Test Summary document to show automated accessibility test has been carried out and that the asset, product or service meets WCAG 2.2 AA guidelines.**

### Assistive Technologies 

Digital assets, products or services must work with assistive technologies. This is so everyone can use the service with the technology they rely on, such as a screen reader or speech recognition software. 

Testing with assistive technology should be part of the overall accessibility testing for the asset / service and should prove that it works with the [minimal following combinations of assistive technologies and browsers as advised by GOV.UK:](https://www.gov.uk/service-manual/technology/testing-with-assistive-technologies) 

| Tool          | Tool Version  | Browser |
| ------------- | ------------- | ------- |
| JAWS (desktop screen reader)  | 2019 or later     | Chrome or Edge (latest version), Firefox 
| NVDA (desktop screen reader)  | Latest            | Chrome or Edge (latest version), Firefox
| VoiceOver on iOS (mobile screen reader)  | Latest | Safari (version 12 or later)
| TalkBack on Android (mobile screen reader)  | Latest | Chrome (latest version)
| Windows Magnifier or Apple Zoom (screen magnifiers)  | Latest  | Any
| Dragon (speech recognition)   | 15 or later          | Chrome (latest version)


In addition to the minimum combinations, VisitScotland is aspiring to enhance accessibility across mobile devices, as more accessible functionality is being in-built into these devices. 

It is recommended that the following combinations are considered:

| Tool          | Tool Version  | Browser |
| ------------- | ------------- | ------- |
| iOS Rotary Controls and Gestures (accessible controls)  | Latest   | Safari (Version 12 or latest) 
| Android Gestures (accessible controls)  | Latest   | Any
| Android Voice Access and iOS Voice control (mobile speech recognition)  | Latest  | Any


### Screen Reader Testing

Screen reader end-to-end testing should be completed to understand how information will be provided to blind or partially sighted users. This testing should follow key user journeys or functionality from start to finish. As sight-impaired users are not able to visually attain information to navigate a digital asset, the following standards should be considered when conducting this type of testing:

- Name, Role, Value

Screen readers will provide information about the role, state and value of user interface components to the user. Native HTML elements, links and components have the capability to provide this information to the screen reading software. Therefore, it is advised to use semantic HTML where possible, and only use ARIA tags in the code where it is strictly necessary to do so. 

If custom controls are created then the [WCAG Name, Role, Value standard best practices](https://www.w3.org/WAI/WCAG21/Understanding/name-role-value.html) should be followed. 


**Descriptive Labels**
If components require input from a screen reader user, clear and unambiguous labels or instructions should be announced to the user. Digital Partners are advised to follow [WCAG 'Labels or Instructions'](https://www.w3.org/WAI/WCAG21/Understanding/labels-or-instructions.html) standard best practices.


**Avoid Repetition of Labels**
When completing a task using a screen reader, if labels are repeated or unrelated information is being read out, then removing elements from the accessibility tree should be considered.

**Keyboard Shortcuts**

Screen reader users can utilise keyboard shortcuts to navigate pages more efficiently. Typical shortcuts involve functions to list all element types available on the page and to skip to the next desired element type. The default shortcuts provided with each screen reader should function as expected.
Additional information on screen reader shortcuts and gestures can be found on the [deque university resource collection](https://dequeuniversity.com/screenreaders/). 

###	Testing Principles

Most users do not amend the settings on their assistive technology and thus Digital Partners are advised to test their software using assistive technologies on their default setting.

It is recommended that screen reader testing is conducted using NVDA over JAWS, as testing should be conducted with the lesser sophisticated product.
Real devices or physical technology should be used if available, though Digital Partners must consider testing on virtual machines, emulators, or cloud-based devices if access to a real device or physical technology is not possible.

When testing using assistive technology, make sure: 
- Users can access information **and**
- Information provided is understandable **and**
- Everything on the interface is usable, or an alternative method is provided.

Finally, VisitScotland recommends accessibility testing beyond compliance. Accessibility is about people and Digital Partners should test to provide the best user experience when using assistive technology and meeting accessibility needs. 

For further guidelines on how to test with assistive technologies, see the [UK Governments 'Testing with Assistive Technology'](https://www.gov.uk/service-manual/technology/testing-with-assistive-technologies) webpage.

**Digital Partners are required to provide VisitScotland with a Test Summary document to show a testing with assistive technology has been carried out. This should include software and version, browser and version, project, task, result, name of tester, date, and details of any errors.**

*Document last review date: 14/05/2025*