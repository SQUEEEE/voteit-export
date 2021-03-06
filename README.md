# voteit-export
Program to take the XML export of a VoteIT-meeting and process it to be imported into a spreadsheet

## Background
The motivation for this program is that in preparation for bigger annual meetings (such as SFSFUM in this case), it is preferable to be able to get an overview of the different proposals. This is usually done manually but for this year we thought we would automate it a bit. 

## XML format in VoteIT-export
```
<Root xmlns="http://voteit.se/printable">
  <AgendaItem>
    <AgendaItem_title>[...]</AgendaItem_title>
    <AgendaItem_body>[...]</AgendaItem_body>
    <AgendaItem_hashtag>[...]</AgendaItem_hashtag>
    <Proposals>
      <Proposal_creator>[Display name (username)]</Proposal_creator>
      <Proposal_text>[...]</Proposal_text>
      <Proposal_aid>[ID of item]</Proposal_aid>
      <Proposal_state>[...]</Proposal_state>
    </Proposals>
    <DiscussionPosts>
    </DiscussionPosts>
  </AgendaItem>
  <AgendaItem>
    ...
  </AgendaItem> 
</Root>
```
