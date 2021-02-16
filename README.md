# Better booking experience - Workstream 2

Use this list to navigate this page:

* **Diagram versions**
    * [Version 1.6](#version-16) updates the flow to reflect two-step document ordering process
    * [Version 1.5.1](#version-151) updates the flow to reflect a new URL approach
    * [Version 1.5](#version-15) incorporates changes in response to the first round of user testing
    * [Version 1.4](#version-14) allows users to see general availability up front and/or select a specific date up-front
    * [Version 1.3](#version-13) extracts the confirmation step to a separate page and accommodates analytics feedback in HTTP parameter options
    * [Version 1.2](#version-12) outlines the pages, proposes URLs, HTTP methods and parameters for passing information
    * [Version 1.1](#version-11) elaborates on some of the features alluded to in Version 1.0
    * [Version 1.0](#version-10) is the flow MVP estimates will be based upon
    * [Version 0.0.8](#version-008) is the flow updated have accessibility questions moved the the end of the process
    * [Version 0.0.7](#version-007) is the flow updated to reflect the feedback to 0.0.6.
    * [Version 0.0.6](#version-006) is the flow updated to reflect some of the feedback to 0.0.5.
    * [Version 0.0.5](#version-005) is the flow updated to reflect some of the feedback to 0.0.4.
    * [Version 0.0.4](#version-004) is the flow developed by Matt B and Gwyn based on their understanding of the systems/process.
* **User testing feedback**
    * [Second iteration](#second-iteration) tested the version 1.5 wireframes
    * [First iteration](#first-iteration) tested the version 1.4 wireframes with six participants
* [Feedback which has not been addressed](#feedback-which-has-not-been-addressed)
* [Estimation table](#estimation-table)

## Introduction

Workstream 2 is intended to improve upon what was delivered under Workstream 1 while acknowledging that it's better to launch sooner and iteratively improve the experience over time than to delay in an attempt to create the ideal experience. We will also need to keep in mind that we're in the process of developing a new technical platform for our website and as a result some of this work will essentially be throwaway so some more complex features will likely be added to our future Beta plans rather than included in Workstream 2. 

The first step of Workstream 2 is analysis of required messaging, decisions and user actions. These are being recorded in flow diagrams and uploaded here for versioning purposes. 

Once a workable high-level flow representing required steps is understood and we have a clear sense of the scope for this work, we will need to estimate the effort involved in delivery. **If estimates exceed available time and resources, we may at this point need to revisit the scope and flow**. There is [a table](#estimation-table) below for recording estimates and related considerations.

Diagrams can be opened in [draw.io](https://draw.io). For each there is also a PDF version. There are also Axure prototypes which have the `.rp` file extension.

## Version 1.6

This [version](iterations/1.6.pdf) updates the flow to reflect the two-step document ordering process.

Changes to the screens include: 

<dl>
    <dt>"there was confusion around 'number of docs needed' and 'add fields' most users expected the number of fields shown to correspond with the number of documents permitted to order"</dt>
    <dd>
        <p>We have addressed this by showing all fields. They are presented on larger screens in four columns.</p>
        <p>We did have a question here: is the series field within the bulk order form necessary? We anticipate it's needed to help identify any added items that are not from the series (and to simplify the necessary validation messages). If so we think it could be made clearer - for example, by saying something along the lines of "Enter the series number. All documents will be checked against this"
    </dd>
    <dt>"much confusion around the  'reserve'  tick boxes in both panes: is a doc only ordered once I tick reserve and the others are just there for later?"</dt>
    <dd>We have addressed this by giving reserves their own fieldset and legend (title).</dd>
    <dt>"make it clear from this page how to get back to this form to amend"</dt>
    <dd>We have added some content which explains this to both the order form and the confirmation page. For the confirmation page there is also a link to 'Edit your order'. This all needs to be reviewed by content speclialsts.</dd>
    <dt>"users understand 'save changes' but some expected an additional page after this with the full, printable, document order and a 'confirm order' button to submit"</dt>
    <dd>It is now a two-step process of editing and reviewing the order. The button text will need to be reviewed by content experts.</dd>
    <dt>"expectation of a time for the deadline for ordering"</dt>
    <dd>We had added a time (and time zone) to the next iteration. Note: this will need some thought regarding the difference between <a href="https://www.gov.uk/when-do-the-clocks-change">GMT and BST</a>.</dd>
    <dt>"most users very happy with ability to amend order until deadline - but some experienced users stated they would not need this"</dt>
    <dd>We don't think this requires any changes to the user interface or flow since it currenlty supports their needs.</dd>
    <dt>"would be good to manage expectations about when doc order is actually confirmed and if this will be in time to choose alternates ( will be told if their docs are already reserved for someone else and if they can add more in that case)"</dt>
    <dd>We have copied over the microcopy from the existing Advance and Bulk Order forms, removing or reordering where appropriate (for example, removing the Privacy Policy statement since these forms no longer capture personal information).</dd> 
    <dt>"there was some confusion around where you would go to get document references - we need express this clearly"</dt>
    <dd>We've added the microcopy from the existing forms which explains this.</dd>
    <dt>"user expect it to be clear if a doc reference has been 'validated'"</dt>
    <dd>We are proposing that a standard validation pattern (as is in place for the existing Bulk and Advance Order forms) would work here. This would be a summary message and individual field messages.</dd>
    <dt>"is there a way to change booking and keep doc order if we are booking 4 weeks in advance and something comes up?"</dt>
    <dd>This seems out of scope for the MVP</dd>
    <dt>"will it be possible to select a seat? when will users be told what seat they have been allocated?"</dt>
    <dd>Seat selection is not within scope for the MVP. The seat will be allocated to the user. The question about when users will be told is to be agreed.</dd>
    <dt>"we will need to clarify comms about next steps for users"</dt>
    <dd>We need to explore this more as a team to understand what is needed.</dd>
</dl>



## Version 1.5.1

This [version](iterations/1.5.1.pdf) is a minor update to reflect back end development decisions about URLs. These changes have been agreed by analytics. 

## Version 1.5 

This [version](iterations/1.5.pdf) incorporates the following changes **in response to user feedback**: 

<dl>
<dt>Make it very clear where to start the process - Users are confused by being able to choose by date and by order type - make it more clear what they need to do in the first step</dt>
<dd>This version invites the user to make a single choice on the first page. Options are presented with equal weighting to make it clear what the two distinct options are. We have changed the visual presentation and added comparative text to help users understand the difference.</dd>
<dt>Allow users to easily start with a date/availability.</dt>
<dd>In order to provide a richer presentation of availability there will be more controls on the interface. This immediately creates more information to process which risks people missing important content. In order to retain the principle of the previous recommendation, we are suggesting that the richer presentation of availability comes once the user has been presented with key information (what they will need etc.) and a user has made a choice about the volume of documents they want to look at.</dd>
<dt>Try to limit the number of pages/steps so if user needs to amend a choice to increase availability they can do it more easily.</dt>
<dd>We have reduced the number of pages from a seven down to four (this includes the confirmation screen).</dd>
<dt>The title of this page is 'Book a Visit' confusing to start with choosing an order type. Refine this to be more about the visit rather than document type.</dt>
<dd>We have updated the page title to be 'Book a visit to view our documents'. We have also updated the options to reflect this with 'Book a standard visit' and 'Book a bulk order visit'. </dd>
<dt>Most users did not notice the reader's ticket or computer booking options - this needs to be reconsidered.</dt>
<dd>We have suggested that 'What you will need to book a visit' is treated as page content - rather than given the visual treatment given to options on the page - and is placed before the booking options on the basis that it has information related to that decision. We have also suggested that the 'PC use only' option is moved below the primary booking options and given a slightly different visual treatment (though we'll need to be careful that it is short).</dd>
<dt>Perhaps less emphasis on Bulk and Map room as these are not as common - not equal choices as currently presented. Instead perhaps show availability by default to the most common type of booking (Standard with Standard reading room  with an option to add a camera stand. You could allow users to change this default view via filters perhaps? Perhaps as well signposting to a separate journey for bulk orders as these are so different.</dt>
<dd>We have suggested addressing this in two ways: firstly by having the 'standard' option visually differentiated from the bulk option with guidance that it is the 'Most commmon choice'. Secondly, the Map room will not be presented as the default option on the availability tool.</dd>
<dt>User needs immediate feedback on choices made and a way to undo/amend easily to increase availability.</dt>
<dd>We have sought to improve the immediate feedback by introducing the date availability tool and </dd>
<dt>Instead of clicking 'next ' or 'refresh' can this happen automatically when user selects the option itself, thus removing an interaction/step?</dt>
<dd>We have moved away from clickable panels (and the 'one idea per page' approach) which should address this issue. It is worth noting though that the core, HTML only version (which will be presented to any user who does not have JavaScript and/or CSS) will require the presence of 'next' or 'refresh' buttons. This version is likely to be encountered by less than 2% of users.</dd>
<dt>All users knew what to expect at the end of this process - an advance order form or an email with confirmation and link to an advance order form so let's keep this similar in next iterations unless we can make this even more seamless.</dt>
<dd>This part of the process has not changed in this iteration but this feedback will be considered in future iterations.</dd>
</dl>

## Team feedback 

It also incorporates changes in response to feedback provided when it was shared with the Digital Services team: 

<dl>
<dt>Indicate that there are many more 'standard' seats than there are 'bulk order' seats</dt>
<dd>We have proposed updating the options presented on the first page to include the number of spaces available for each.</dd>
<dt>Add version of availability which demonstrates how no availability is shown</dt>
<dd>...</dd>
<dt>Provide hint of user's email address on confirmation page</dt>
<dd>We have proposed updating the Reader's Ticket entry page to allow users to see a hint of the email address associated with their Reader's Ticket before submitting the form. Note: there may be broader implications of this which we need to discuss as a team (for example, what's the process for changing an email address associated with a Reader's Ticket; what do we say to users who see their email address is wrong)</dd>
<dt>User indicated it would be helpful if there was a way for them to change the email address associated with their Reader's Ticket</dt>
<dd>We expect this is beyond MVP</dd>
</dl>

Additional notes on Version 1.5: 

* We have tried to simplify the interface on the date availability page and to make it more touch device friendly.
* By describing the distinction between a bulk and standard order it has removed the need for a description on the date availability too. This has allowed us to introduce a control which allows users to toggle between the views without cluttering the interface or having to provided additional explanation. 
 * We have proposed a way for two-day visits to be presented in the availability presentation tool
* We have tried to simplify the interface on the reader's ticket page and to focus attention on the primary action.


## Version 1.4

This [version](iterations/1.4.pdf) seeks to address what has been described as the 'availability conundrum', the essence of this conundrum is: **_how do you present general availability (in a meaningful and digestible way) when availability is any combination across five facets (date, room, order type, camera stand and duration)?_** Previous approaches have have either: 

* led the user through a process of stating their requirements across each facet (which provides the user with a clear sense of the places available for your needs but does not address the question of showing availability up front); 
* shown general availability up front in which case the availability shown is unlikely to reflect any specific user requirements and may lead to frustration later; 
* shown availability based on some 'defaults'. This could lead to users missing that there is availability beyond that which is shown and introduces complexity when the default availability has been exhausted

The approach in version 1.4 attempts to strike a balance between both by introducing 'specified' and 'unspecified' date paths.

It also: 

* Clarifies the requirement for a timer on the Reader's Ticket page (and how this will be approached in order to meet accessibility regulations)
* Removes the confirmation page on the basis that it doesn't fit with a user experience where an order remains open for a user to amend at any point until it is closed (by the system, at a specified point before the visit) so that Document Services can prepare the order. Instead the user will be provided with in page confirmation of any amendments they make. 

## Version 1.3

This [version](iterations/1.3.pdf): 

* extracts the confirmation step to a separate page 
* accommodates analytics feedback in HTTP parameter options

## Version 1.2 

This [version](iterations/1.2.pdf): 

* Outlines the pages included in the application
* Proposes URLs, based on a to be define service name
* Proposes HTTP methods and parameters
* Elaborates on [progressive enhancement options](https://github.com/nationalarchives/ds-booking-experience#estimation-table) for the availability tool

## Version 1.1 

This [version](iterations/1.1.pdf): 

* Elaborates on [post booking actions](post-booking-actions.md) that will be automated in the system (reminder emails etc.)
* Adds questions relating to the scenario where a user might not have access to the email address associated with their Reader's Ticket
* Extends the flow to allow users to cancel their visit

## Version 1.0

This [version](iterations/1.0.pdf) was presented to stakeholders along with the MVP requirements and an accompanying [Axure prototype](/iterations/1.0.rp) (see screenshots [here](/iterations/wireframe-screenshots/1.0)) on 17 December. This major version bump reflects agreement that this is an initial version to be estimated against (accepting that further refinement and thought will be necessary).

## Version 0.0.8 

This [version](iterations/0.0.8.pdf) has been updated to move questions related to accessibility needs to the end of the process. 

## Version 0.0.7

This [version](iterations/0.0.7.pdf) has been updated to reflect feedback received on 10 December. 

### Changes in response to feedback for 0.0.7

| Feedback  | Has it been addressed in this iteration | How it has been addressed  |
|---|---|---|
| **Filter place availability up front:** allow users to filter availability (so that they can see if there's a suitable place for them) | Yes | Very early in the process (on the first screen) users can filter places by specific attributes (two-day visit, bulk or advance order, camera stand, specified reading room) |
| **Hold a place:** allow users to hold a place (once they have identified a suitable place) | Yes | Having identified a suitable place users can immediately hold it for a (to be specified) period. The booking will be confirmed when they provide their Reader's Ticket |
| **Allow document orders to be edited:** this would allow document orders to be edited before submission to document services | Yes | Users are able to return to the form at any point (authenticating using a unique code and their Reader's Ticket) in order to make an amendment. The form is only sent to Document Services when it is necessary to begin preparing the documents. This is a slightly different model in that the user will be _saving_ their order rather than _submitting_ it |
| **Ordering up to 24 documents is problematic:** it could be misleading since it is only available to users who are making multi-day visits | Yes | We have removed this option. The user can now filter by availability at the beginning of the process and will be presented with a form that reflects their choice. **Note:** this does require the forms to be somewhat dynamic in order to accommodate multi-day visits |

## Version 0.0.6

This [version](iterations/0.0.6.pdf) has been updated to reflect, where possible, the stakeholder feedback received on 4 December. We've also prepared a flow to represent the logic to determine if a user is [within the maximum number of bookings](within-max-bookings.pdf).

### Changes in response to feedback for 0.0.6

| Feedback  | Has it been addressed in this iteration | How it has been addressed  |
|---|---|---|
| **PC and document visits:** users may want to use both PCs and to view documents in the same visit | Yes | Explain that users booking to view physical documents will be able to user PCs in the 'Start here' area but those who do not wish to view documents need not proceed through this booking process (providing link to relevant page on our site) |
| **PC seats are not bookable:** they're located in the 'Start here' area | Yes | See above|
| **Transparency about impact of selected options:** ideally the user should transparency about how their choices affect availability - e.g. what happens if I select camera stand or do not? | Yes | We have proposed two things here. The first is to show the availability at point of selection (For example, when selecting a reading room, the number of seats will be shown). The second is to allow the user to step back to a previous step should they wish to. |
| **Key questions for seat allocation:** which reading room; camera stand; accessibility requirements | Yes | We have introduced these three options. For camera stand and reading room choices, the number of spaces will be shown. Again, users will be able to step back to an earlier decision. | 
| **Avoid advising on number of days:** we should seek to avoid a situation where staff have to tell a user that they are unable to return the next day when they haven't concluded their research and the duration of the visit was based on our advice. | Yes | We have removed the recommendation. The user selection will instead be used to determine if they are shown the bulk or advance order form. |


## Version 0.0.5

[Version 0.0.5](iterations/0.0.5.pdf) was concluded on 3 December (before a workshop on 4 December). It incoporates some of the feedback Version 0.0.4 received, as detailed below. All feedback which has not yet been addressed is [listed below](#feedback-which-has-not-been-addressed). We have also prepared a flow representing the [current seat selection process (in Elsa)](elsa-diagram.pdf).

### Changes in response to feedback for 0.0.5

| Feedback  | Has it been addressed in this iteration | How it has been addressed  |
|---|---|---|
| **Users who need PC access only**: The flow should accommodate users who use reading room PCs to access online resources. These users will not need a reader's ticket or to order documents. | Yes | We think there are two options here. The first would be to have this as a totally separate journey from the 'Visit us' page. If we were to opt for this we could signpost to that from the introduction. The second option would be to have this as an early choice in this process where a user is asked which path they'd like to go down. We think the latter probably makes most sense because there are more options to provide the necessary information. |
| **2 consecutive day visits**: These are not confined to users making a bulk order. They can also be for people who want two consecutive days of advance orders. | Yes | We have updated the flow to provide a suggested number of days to visit (based on the number of documents ordered) and also allowed users to override this with their own duration selection |
| **Flexibility for multi-day visits**: There should be some flexibility to allow for, say, 3 day visits should that option become available in future. | Yes | We have updated the flow to provide a suggested number of days to visit (based on the number of documents ordered) and also allowed users to override this with their own duration selection | 
| **Should we provide guidance based on probable need?** This would involve determining how many days are _probably_ needed (based on the number of documents ordered) then showing the user availability and letting them choose. | Yes | We have updated the flow to provide a suggested number of days to visit (based on the number of documents ordered) and also allowed users to override this with their own duration selection | 
| **Link in to Elsa**: Because the Elsa frontend is written in Flash (which is end of life) this should link in with Elsa meaning it would have real long-term viabiity. | Yes | In addition to selecting a specific seat Elsa allows users to indicate: types of documents they are likely to be viewing (maps, pre-1688 etc.), location preferences (window proximity), various access needs (difficulty bending down or wheelchair access), researching with others etc. James B has pulled together a [decision tree](elsa-diagram.pdf) which shows the current options provided in Elsa. While the seat selection is stored in Doris, new work (based on a like-for-like implementation) that would be required includes: the front-end web application logic to carry a user's state across different screens (and present only logical next steps, based on their previous selections) and pass this through to Doris; a seat selection tool (HTML progressively enhanced to SVG) with element state being linked to Doris availability. |
| **Camera stand availability**: This might be a deal-breaker for some people - should we ask the question earlier. | Yes | We believe we've addressed this by showing the availability of different seat types (including those with camera stands) as an early step in the process. |
| **Build in flexibility**: Build the system so that we can modify quite easily how many consecutive days someone can book for | Yes | We have updated the flow to provide a suggested number of days to visit (based on the number of documents ordered) and also allowed users to override this with their own duration selection |
| **Availability on first page**: By showing availability of the first page will users expect to click on the options shown. | No | This is something we'll need to address through the visual design to ensure the listing is not presented as an interactive element. |
| **Readers ticket - third option**: It is possible a user might have a readers ticket but that it has expired. | Yes | We have updated the flow so that this is reflected in the readers ticket validation process | 

## Version 0.0.4 

[Version 0.0.4](iterations/0.0.4.pdf) was concluded on 25 November in preparation for a stakeholder meeting.

## Feedback which has not been addressed

### Version 0.0.5

* **Don't diminish the experience:** must check for functionality that is provided in Eventbrite that we don't want to lose (e.g. cancellation)
* **Flexibility to changes:** must be able to accommodate changes as COVID situation and offer changes
* **Must be an improvement for DSD manual backend processes**
* **Cancellation option:** is it possible to cancel one day out of a three day visit, for example, without losing the whole visit
* **Amend document order:** is it possible for users to amend a document order in advance of their visit
* **Future proofing:** how far in the future do we need to think about the system? Flexibility e.g. to enable booking of other spaces, PC only spaces, exhibitions etc. 
* **DSD notified once:** can DSD receive a single notification of a booking (rather than multiple notifications for a single booking)
 
### Version 0.0.4

* **Onsite vs online**: We need to consider different flows depending on the user being onsite or online. 
* **Open with 'Choose your date'**: Can we have choose your date at the very beginning of the journey?  
* **Hold the seat**: We need to hold the seat for people while they complete the process 
* **Temporary reader's tickets**: Temporary reader's tickets expire after 6 weeks. Is there potential for a user's temporary ticket to expire before they can get a place? How would we accommodate this. One option could be to look into extending the time for temporary reader's tickets
* **Alternative availability**: If there is nothing available for the user as a result of their stated preferences (for example, a camera stand) we should show them what is available instead (for example, there are seats without a camera stand) 
* **Register needs in advance**: Can users register their needs in advance so that availability which is specific to their needs can be shown up front (Note: this might require a link to a user account which is a bigger project) 
* **Knowledge at first screen**: Does a user necessarily know their document needs when they arrive at the first screen? Might we need to have 'basket' type functionality in Discovery 

## User testing feedback

## Second iteration

This user testing was against version 1.5 of the wireframes. Recommendations were made for each page and added to the [Miro board](https://miro.com/app/board/o9J_lfhjfK4=/?moveToWidget=3074457354146464929&cot=14). 

Actions in response to these recommendations can be found [here](actions-in-response-to-second-iteration-ux-recommendations.md).

## First iteration

This user testing was against version 1.4 of the wireframes with six participants. Recommendations are: 

1. Make it very clear where to start the process - Users are confused by being able to choose by date and by order type - make it more clear what they need to do in the first step
2. Allow users to easily start with a date/availability.
3. Try to limit the number of pages/steps so if user needs to amend a choice to increase availability they can do it more easily.
4. The title of this page is 'Book a Visit' confusing to start with choosing an order type. Refine this to be more about the visit rather than document type.
5. Most users did not notice the reader's ticket or computer booking options - this needs to be reconsidered.
6. Perhaps less emphasis on Bulk and Map room as these are not as common - not equal choices as currently presented. Instead perhaps show availability by default to the most common type of booking (Standard with Standard reading room  with an option to add a camera stand. You could allow users to change this default view via filters perhaps? Perhaps as well signposting to a separate journey for bulk orders as these are so different.
7. User needs immediate feedback on choices made and a way to undo/amend easily to increase availability.
8. Instead of clicking 'next ' or 'refresh' can this happen automatically when user selects the option itself, thus removing an interaction/step?
9. All users knew what to expect at the end of this process - an advance order form or an email with confirmation and link to an advance order form so let's keep this similar in next iterations unless we can make this even more seamless.


# Estimation table

On 27 January the estimation table was moved to Miro and can be found at the right hand side of [this board](https://miro.com/app/board/o9J_lfhjfK4=/)
