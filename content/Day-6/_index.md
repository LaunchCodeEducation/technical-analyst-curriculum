---
title: 6. Technical Writing 
weight: 106
---

## Technical Writing ( Day 1 )
> _“ If everyone is moving forward together, then success takes care of itself “_ –Henry Ford
***

What is Technical Writing? It is the crafting of technical content that provides detailed steps on how to approach and solve a problem. The importance of documentation in engineering lies in knowledge preservation and sharing. When members of our team encounter unfamiliar systems or technologies, they can refer to the documentation to gain a better understanding of how the system functions. More significantly, they can formulate questions about the functionality of methods and design plans based on their existing knowledge.

Many organizations have already documented their processes, design plans, technical architecture, and logical and physical designs. Our task is to familiarize ourselves with this documentation and have our colleagues help fill in any knowledge gaps as we become better acquainted with the systems and workflows within the organization.

Documenting customer interactions and support calls is a valuable form of documentation that aids in sharing the knowledge acquired during a call with other team members throughout a workweek. This enables them to review our notes and determine the next logical steps to resolve the issue without retracing previously taken steps. Writing effective technical documentation, user manuals, or call notes follows a consistent process that includes, but is not limited to:

- Formatting and organizing documentation for clarity.
- Reviewing and editing documentation for accuracy and completeness.
- Understanding our audience (readers).
- Utilizing visual aids.
- Providing step-by-step instructions and conditional callouts.

## Writer's Framework

Our initial steps involve establishing the framework for our documentation. We determine the subject matter, the target audience, and the key information we intend to convey before commencing the writing process. This framework is universally applicable and can be employed for creating presentations, research papers, as well as fiction and non-fiction pieces.

1. Who is the intended audience for this document?
2. When should they refer to this document, and what should it contain or omit?
3. What is the document's topic?
4. How can the readers utilize the information provided?
5. Identify the key points or objectives.

## Situation: Using the Writer's Framework for Password Reset

**Password reset for a customer** is one of the most common issues encountered by help desks. It is also one of the simplest to resolve. Let's walk through an example using this framework. Imagine working in a call center with a note-taking application for call notes and a knowledge management system for research. You, as a Technical Service Analyst, receive a call for a password reset.

**Note:** This example pertains to smaller organizations. Larger organizations may use multiple knowledge management systems and two or three ticketing systems for issue reporting. For our illustration, we will keep things straightforward.

### Who Needs to Read This Document

There might be two distinct audience members for this document: Tier 1 Help Desk and Tier 2 Support. Therefore, we should include relevant screenshots and notes for each team's review. As learned from [Module 1: Effective Communication]({{< relref "../Day-1/_index.md" >}}), we can gather additional information by asking open-ended questions about the reported issue and actively listening to identify broader issues. For instance, if a caller reports encountering a 404 error multiple times while trying to log in, which resolved after the fifth attempt upon refreshing the browser, this may signify an issue with application routing and warrant escalation to the network or application team for further analysis.

### When Should They Read This Document

This document serves as a reference guide for performing password resets at the Tier 1 support level. It does not cover changing a user's login name/details or account information. If the user requires steps other than a password reset, they should be escalated to Tier 2 Support.

###  What Is the Document About

This section details the proper steps for authenticating and verifying a user before resetting their password. It includes the necessary firewalls to log in, the application for password reset, and how to confirm successful password changes. Additionally, this section provides information on self-service steps for users to reset their own passwords.

### How Can They Use This Information Going Forward

Technical analysts can streamline the steps and collaborate with the development team to implement a self-service solution for users to reset their passwords using a self-hosted application.

### Identify Key Points or Objectives

The document's purpose is to reduce the Mean Time To Respond (MTTR) for password reset calls by outlining the required steps for Technical Analysts to complete this task.

## Learner Profile (Technical, Non-Technical)

When creating technical documents, we often cater to both technical and non-technical users. In such cases, it's essential to adjust our approach for explaining complex technical concepts and design presentations. We should avoid using industry-specific jargon, which may not be understood by individuals outside the field. Visual aids, such as charts, can enhance our message's clarity. Our audience may include developers, engineers, or executive leadership teams (e.g., Vice Presidents, Chief Executive Officers), so it's crucial to ensure that our content is comprehensible and not bogged down by technical terminology.

1. Does anyone in your audience possess prior knowledge of the content in your presentation?
2. Will there be Subject Matter Experts (SMEs) present?

If either of the above questions holds true, we should address their potential concerns and consider involving SMEs in the presentation. We must focus on storytelling rather than providing mere bullet points or text on the screen or in an email. Additionally, we should pay attention to font size, making sure it's readable for all team members, including those with color blindness or those who wear glasses. If we use color highlighting, it's advisable to explain its significance. Accessibility standards should be considered, including but not limited to:

- Font size
- Color usage
- Language
- Proper headings
- Text readability
- Image alternative text

For web-based documentation, you can explore [web accessibility](https://www.w3.org/WAI/standards-guidelines/wcag/), and it's important to be aware of other accessibility aspects in the documentation created for a broader audience.

## Presentation and Visual Impact 

> “ I hate it when people use PowerPoints instead of thinking. People confront a problem by creating a presentation. I want them to engage,  hash things out at the table, rather than show a bunch of slides. People who know what they’re talking about don’t need PowerPoint.” – Steve Jobs

Although Steve Jobs and Jeff Bezos discouraged the use of PowerPoints, many organizations still rely on this form of communication for various reasons. One of the most crucial aspects to consider is the color palette. It's a good rule of thumb to use approved colors or those similar to what we've seen in other presentations within the organization. Often, the marketing team has already developed templates for both internal and external communications. When deciding on colors, select three to four main colors for the following areas:

1. Text,
2. Headings,
3. Shapes/Images, and
4. Callouts.

When creating presentations, it's important to keep the text concise and supplement it with images. Make sure the text is large enough for everyone in the room to see, especially those at the back. Focus on engaging your audience through calls to action and visual callouts. 

For instance, consider a sales chart covering a year, where one month significantly affects the total. You can highlight the problematic month in red and use a lighter pink for other areas to draw attention to the key point of the slide. This highlighting can spark questions or become the main talking point. 

Keep in mind that external factors can impact your data. If, for example, you're looking at iPhone sales data, you might notice a spike in December. Does this mean people bought iPhones for Christmas gifts? 

Also, think about what's missing, like data on different cell phone providers. We might not know which provider was most successful that year. Are all providers doing well during the holidays, or just one? 

It's crucial to report diligently, especially because your slides may be shared with teams, departments, or the public. Prepare to answer questions by setting aside 10-15 minutes for a Q&A at the end of your presentation. Some people may wait until the end to ask questions, as they want the full picture before discussing it further.

{{% notice green "Protip" "rocket" %}}
Turn failure into stepping stones. Don’t be afraid to show what you learned or where the project failed. This can help others engage in the conversation or get involved in the conversation or project. 
{{% /notice  %}}

{{% notice green "Protip" "rocket" %}}
Try to send the presentation to the group ahead of the meeting at least 24 hours at most 72 hours in advance to allow people time to review the deck before the meeting.  
{{% /notice %}}

