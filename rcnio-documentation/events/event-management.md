# Event Management

Event management is very easy. If you can edit text files—you can manage events. After first few updates it would feel easier than current system. So lets see how to do it.

Management of events consists of the following operations \(in the order of frequency\):

* editing of the existing event
* creating a new event
* moving / canceling existing event

## Prerequisites

Login at github.com with your account \(TK paste account name\)

## Technical info

All events are stored in a text format, this allows for a great flexibility and a fast iteration. Very soon this will change since Anton is currently building a state of the art admin interface, so it will be even easier.

## Editing of the existing event

Lets do a particular task, say we want to update a name for Oakland Grand Prix and add a permit number to it.

\* open the following URL \(TK url to 2017 events file\)  
\* press ctrl+f \(cmd+f on mac\) and type "Oakland Grand Prix", you should be able to find the event:

\(TK screen shot\)

\* from now on it should be pretty obvious where to make the name change, go ahead and change the name to "NCNCA Criterium Championships: Oakland Grand Prix"  
\* to add a permit, we would need to add a new property to the event, just like with name as you can see, everything is in the format:

`"propertyName": "property value"`

TK: permit is added by defining a property:

`"usacPermit": "2017-1234",`

notice `,` at the end, it is required for every name-value pair. So let's go ahead and define it.

\* after your are done add a message to this box, summarizing your changes:

TK &lt;screen shot of the box&gt;

and press "crate pull request"

That is it. I will automatically get notified about that and will review and apply your changes. Please note, that this review process is temporary and you won't have to go through it in the future when you will feel comfortable making changes.

## Creating a new event

The process of creation of most of the events is streamlined. Current process at the beginning of the year is the following:

\* promoters collaborate in google spreadsheet on the future calendar

\* when they are done webmaster is asked to create a new Calendar

\* it takes day or even few days to fill it out since it's typically 100+ events

With the new calendar this changes to:

\* promoters collaborate in google spreadsheet on the future calendar and it's immediately connected to a new system as a "calendar draft". \(TK: paste an example of that for 2016\)

\* when they are done, webmaster can turn that draft into a published calendar in 5 minutes! No manual entry is needed at this point

So we would need to create only events that were not planned initially. Those typically include nationals, Tour of California, NCNCA Board Meetings and re-scheduled events. Let's see how to do it.

To simplify this process I built an admit tool which you can access here:

[https://rcn.io/admin/create-event](https://rcn.io/admin/create-event)

It pre-populates event with all required properties and let's you see how event looks like in realtime!

