The Demo Fire Door Inspection PowerApp requires two SharePoint lists named 'RoomStock' and 'Inspection'.

Users of the app can be given Read access on the 'RoomStock' list and Edit access on the 'Inspection' list. It is recommended that the Inspection list would have a custom permission level applied to protect the data from being manipulated directly if it were to be utilised in a production environment.

The lists require the following custom columns:

RoomStock

Site (Text)
Area (Text)
Block (Text)
SubBlock (Text)
Room (Text)

Inspection

InspectionDate (Date and time)
Site (Text)
Area (Text)
Block (Text)
SubBlock (Text)
Room (Text)
Handle (Choice)
Lock (Choice)
Closer (Choice)
Hinges (Choice)
Brushstrip (Choice)
Gap (Choice)
Frame (Choice)
Signage (Choice)
Keeper (Choice)
Letterbox (Choice)
NextDueDate (Date and time)


Import the app following the process described in the Microsoft documentation: https://github.com/MicrosoftDocs/powerapps-docs/blob/main/powerapps-docs/maker/canvas-apps/export-import-app.md

Remove the references to the data sources in the app and replace them with your own SharePoint lists.
