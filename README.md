# Better booking experience - Workstream 2

Use this list to navigate this page:

* Diagram versions
    * [Version 0.0.5](#version-005) is the flow updated to reflect some of the feedback to 0.0.4.
    * [Version 0.0.4](#version-004) is the flow developed by Matt B and Gwyn based on their understanding of the systems/process.
* [Feedback which has not been addressed](#feedback-which-has-not-been-addressed)
* [Estimation table](#estimation-table)

## Introduction

Workstream 2 is intended to improve upon what was delivered under Workstream 1 while acknowledging that it's better to launch sooner and iteratively improve the experience over time than to delay in an attempt to create the ideal experience. We will also need to keep in mind that we're in the process of developing a new technical platform for our website and as a result some of this work will essentially be throwaway so some more complex features will likely be added to our future Beta plans rather than included in Workstream 2. 

The first step of Workstream 2 is analysis of required messaging, decisions and user actions. These are being recorded in flow diagrams and uploaded here for versioning purposes. 

Once a workable high-level flow representing required steps is understood and we have a clear sense of the scope for this work, we will need to estimate the effort involved in delivery. **If estimates exceed available time and resources, we may at this point need to revisit the scope and flow**. There is [a table](#estimation-table) below for recording estimates and related considerations.

Diagrams can be opened in [draw.io](https://draw.io). For each there is also a PDF version. There are also Axure prototypes which have the `.rp` file extension.

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
* **Temporary reader's tickets**: Temporary reader's tickets expire after 6 weeks. Is there potential for a user's temporary ticket to expire before they can get a place? How would we accommodate this. One option could be to look into extending the time for temporary reader's tickets | | |
* **Alternative availability**: If there is nothing available for the user as a result of their stated preferences (for example, a camera stand) we should show them what is available instead (for example, there are seats without a camera stand) 
* **Register needs in advance**: Can users register their needs in advance so that availability which is specific to their needs can be shown up front (Note: this might require a link to a user account which is a bigger project) 
* **Knowledge at first screen**: Does a user necessarily know their document needs when they arrive at the first screen? Might we need to have 'basket' type functionality in Discovery 

## Estimation table

| Specialism | Confidence in understanding of what is required | High-level estimate of dedicated effort required | Confidence in this estimate | Further information that would help with estimating | 
|---|---|---|---|---|
| Testing effort (all required types) ||||
| UX effort ||||
| Content design effort ||||
| Analytics effort ||||
| Reporting effort ||||
| Server-side development effort ||||
| Front end development effort |||| To provide a high-level estimate for front end development aspects of Workstream 2 as a whole we need: a clear understanding of the scope; an agreed flow to base estimates on, and; an understanding of how the flow corresponds to user interfaces to be built. We also need to know if any of the other approaches will impact this (for example, if it is anticipated we'll need to write any JavaScript modules to support the analytics approach) and how many iterations of user testing / refinement are expected (since each iteration will add to the estimate).
| Design effort ||||
