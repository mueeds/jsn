```JSON
{
   "$schema": "http://columnformatting.sharepointpnp.com/columnFormattingSchema.json",
   "elmType": "div",
   "style": {
      "display": "inline-flex",
      "align-items": "center"
   },
   "children": [
      {
         "elmType": "div",
         "style": {
            "width": "100%",
            "display": "=if(@currentField != '', 'none', 'block')"
         },
         "txtContent": "*****"
      },
      {
         "elmType": "div",
         "style": {
            "width": "100%",
            "display": "=if(@currentField != '', 'block', 'none')"
         },
         "txtContent": "[$currentField]",
         "attributes": {
            "title": "Click the eye icon to reveal the hidden value"
         }
      },
      {
         "elmType": "div",
         "style": {
            "margin-left": "8px",
            "cursor": "pointer"
         },
         "txtContent": "👁️",
         "customRowAction": {
            "action": "executeFlow",
            "actionParams": "{\"id\":\"YourFlowID\"}"
         },
         "attributes": {
            "title": "Click to reveal hidden value"
         }
      }
   ]
}
```
