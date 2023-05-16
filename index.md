<p align="center">
<img src="https://raw.githubusercontent.com/wsg-ariadne/ariadne/main/public/assets/logo.svg" width="200" alt="ariadne">
</p>

**Version history**

Version 1.1 (2023 May 16)
- Added the Ariadne logo and a Table of Contents
- Properly formatted the [Collection of Information](#collection-of-information) section
  - Due to a formatting error, the section header was incorrectly merged into the last paragraph of [Overview of Functionality](#overview-of-functionality). This has now been fixed.
- Updated [Overview of Functionality](#overview-of-functionality) to match the functionality of Ariadne as of version `0.1.2 (20230514 main@d6ecb34)`
  - The Extension now attempts to perform automatic Classification whether or not the URL of the web page that you are visiting is in the database of sites reported to use deceptive design patterns. This is now reflected in this section.
  - The Extension displays the Classification results for the Candidate text and Screenshot, in addition to the report statistics for the URL, in the Extension user interface. This is now reflected in this section.
- Updated [Collection of Information](#collection-of-information) to match the functionality of Ariadne as of version `0.1.2 (20230514 main@d6ecb34)`
  - Because the Extension is designed to work in the background, we made it clear that information is collected automatically and cannot be disabled for as long as the Extension is installed and enabled.
  - Version `0.1.2 (20230514 main@d6ecb34)` of the Extension adds the ability to submit a Report containing feedback on the results of the automatic Classification. We added a section describing the information we collect on Reports.
- Added a section on [Anonymity](#anonymity)
  - Ariadne is anonymous by design, in that we do not require you to log in or otherwise identify yourself to be able to use the Extension. We have made this explicit by adding this section.

Version 1.0 (2023 May 14)
- Initial version

# Privacy Policy

This Privacy Policy explains how the Ariadne research team ("we," "us," or "our") collects, uses, and shares your information when you use our browser extension ("Extension").

- [Privacy Policy](#privacy-policy)
  - [Overview of Functionality](#overview-of-functionality)
  - [Collection of Information](#collection-of-information)
    - [Basic Functionality](#basic-functionality)
    - [Reporting Functionality](#reporting-functionality)
    - [Use of Information](#use-of-information)
  - [Anonymity](#anonymity)
  - [Security](#security)
  - [Changes to this Privacy Policy](#changes-to-this-privacy-policy)
  - [Contact Us](#contact-us)


## Overview of Functionality

The Extension communicates with a remote server (“Server”), which is responsible for performing the machine learning classification (“Classification”) and managing the deceptive design reports (“Report,” “Reports”), submitted by users like you.

To notify you of any possible deceptive design patterns on the pages you visit, the Extension works by getting the URL of the web page that you are visiting. It then executes the following actions:

1. Check that URL against a database of sites reported to use deceptive design patterns;
2. Perform automatic Classification by:
   1. Looking for candidate cookie banner elements (“Candidate,” “Candidates”) on the web page;
   2. Taking a screen capture (“Screenshot,” “Screenshots”) of the first matching Candidate whose text contains any of the words “cookies,” “consent,” or “tracker,” all of which are words usually present in cookie banner text;
   3. Extracting the text present in the Candidate;
   4. Sending the Screenshot and the extracted text to the Server for Classification.

Candidates are elements that float and do not move (i.e., a CSS `position` value of `sticky`, `absolute`, or `fixed`, and a positive non-zero `z-index` value), and are thus candidates for being cookie banners.

The results of this process (report statistics for the URL and the Classification results for the Candidate text and Screenshot) are then displayed to you in the Extension user interface.

## Collection of Information

We take your privacy seriously. In this section, we describe what information we collect, how we collect it, and how we use it.

### Basic Functionality

When you install and enable our Extension, we collect, **but not store,** the following information:

- The URLs of the web pages that you visit;
- Screenshots and text content of Candidates detected on the web pages that you visit.

The collection of this information is automatic. It does not require user interaction to occur, and it cannot be disabled, as it is necessary for the basic functionality of the Extension.

As part of the basic functionalities of the Extension and the Server software, which includes logging and maintenance, we may also collect and store the following information:

- The time and date of your visits;
- The browser you're using;
- The operating system you're using;
- Your IP address.

### Reporting Functionality

When you submit a Report using the Extension using

1. the Thumbs Up (“Report correct detection”) button;
2. the Thumbs Down (“Report incorrect detection”) button; or
3. the “Report deceptive design on this page” button;

we additionally collect **and store** the following information:

- The URL of the web page being reported;
- The date and time of your report submission;
- Your rating of the automatic detection, represented by the button you clicked (i.e., Thumbs Up for "correct detection," or Thumbs Down for "incorrect detection");
- A description of the deceptive design pattern that you are reporting, if present.

Should you choose to include them, we also collect **and store** the following supplementary materials ("Attachments") for your report:

- The Screenshot of the Candidate detected on the web page that you are reporting;
- The text content of the Candidate detected on the web page that you are reporting.

These Attachments, although automatically captured and prepared on your device, are not collected or stored by the Server until you explicitly submit them with your Report.

### Use of Information

We use the information we collect to:

- Provide you with the basic functionality of the Extension;
- Improve our Extension's functionality and performance;
- Provide you with a better user experience;
- Understand how our Extension is being used.

We do not sell or rent information to third parties. However, we may share information with third-party service providers who help us operate our Extension or improve our products and services. These third-party service providers are bound by confidentiality agreements and are not permitted to use the provided information for any other purpose.

We may also share collected information in response to a subpoena, court order, or other legal requirement.

## Anonymity

The Extension does not require you to log in or to otherwise identify yourself before use.

All of the information we collect and store, as described in [Collection of Information](#collection-of-information), including any Reports you might submit, are collected anonymously and is not linked to any personally identifiable information.

## Security

We take reasonable measures to protect your information from unauthorized access, use, or disclosure. However, we cannot guarantee the security of your information, as no method of transmission over the Internet or method of electronic storage is 100% secure.

## Changes to this Privacy Policy

We may update this Privacy Policy from time to time. If we make material changes to this Privacy Policy, we will notify you by posting a notice on our website or by posting a notice visible from within the Extension user interface.

## Contact Us
If you have any questions or concerns about this Privacy Policy, please contact us at [ariadne@dantis.me](mailto:ariadne@dantis.me).
