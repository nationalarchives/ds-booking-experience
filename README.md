# Better booking experience 

This repository contains versioned flow diagrams for workstream 2 of the better booking experience.

Diagrams can be opened in [draw.io](https://draw.io). For each there is also a PDF version.

# Versions

* [Version 0.0.4](diagrams/0.0.4.pdf) is the flow developed by Matt B and Gwyn based on the system

## Supplementary documents

* [Elsa diagram](Elsa_diagram.pdf) is a flow chart of existing seat selection functionality in Elsa.

## Feedback to version 0.0.4

| Feedback  | To be addressed in next iteration  | How it has been addressed  |
|---|---|---|
| **Users who need PC access only**: The flow should accommodate users who use reading room PCs to access online resources. These users will not need a reader's ticket or to order documents. | Yes | We think there are two options here. The first would be to have this as a totally separate journey from the 'Visit us' page. If we were to opt for this we could signpost to that from the introduction. The second option would be to have this as an early choice in this process where a user is asked which path they'd like to go down. We think the latter probably makes most sense because there are more options to provide the necessary information. |
| **Temporary reader's tickets**: Temporary reader's tickets expire after 6 weeks. Is there potential for a user's temporary ticket to expire before they can get a place? How would we accommodate this. One option could be to look into extending the time for temporary reader's tickets |||
| **2 consecutive day visits**: These are not confined to users making a bulk order. They can also be for people who want two consecutive days of advance orders. |||
| **Flexibility for multi-day visits**: There should be some flexibility to allow for, say, 3 day visits should that option become available in future. ||| 
| **Should we provide guidance based on probable need?** This would involve determining how many days are _probably_ needed (based on the number of documents ordered) then showing the user availability and letting them choose. ||| 
| **Link in to Elsa**: Because the Elsa frontend is written in Flash (which is end of life) this should link in with Elsa meaning it would have real long-term viabiity. | Yes | In addition to selecting a specific seat Elsa allows users to indicate: types of documents they are likely to be viewing (maps, pre-1688 etc.), location preferences (window proximity), various access needs (difficulty bending down or wheelchair access), researching with others etc. James B has pulled together a [decision tree](Elsa_diagram.pdf) which shows the current options provided in Elsa. While the seat selection is stored in Doris, new work (based on a like-for-like implementation) that would be required includes: the front-end web application logic to carry a user's state across different screens (and present only logical next steps, based on their previous selections) and pass this through to Doris; a seat selection tool (HTML progressively enhanced to SVG) with element state being linked to Doris availability. |
| **Onsite vs online**: We need to consider different flows depending on the user being onsite or online. |||
| **Camera stand availability**: This might be a deal-breaker for some people - should we ask the question earlier. |||
| **Open with 'Choose your seat'**: Can we have choose your seat at the very beginning of the journey? ||| 
| **Build in flexibility**: Build the system so that we can modify quite easily how many consecutive days someone can book for |||
| **Hold the seat**: We need to hold the seat for people while they complete the process |||
| **Alternative availability**: If there is nothing available for the user as a result of their stated preferences (for example, a camera stand) we should show them what is available instead (for example, there are seats without a camera stand) |||
| **Register needs in advance**: Can users register their needs in advance so that availability which is specific to their needs can be shown up front (Note: this might require a link to a user account which is a bigger project) |||
| **Knowledge at first screen**: Does a user necessarily know their document needs when they arrive at the first screen? Might we need to have 'basket' type functionality in Discovery |||
| **Readers ticket - third option**: It is possible a user might have a readers ticket but that it has expired. ||| 
| **Availability on first page**: By showing availability of the first page will users expect to click on the options shown. |||
