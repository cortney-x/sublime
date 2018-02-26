# sublime
### Emmet
```
[
    { "keys": ["super+shift+c"], "command": "duplicate_line" },
    {
      "keys": ["tab"], 
      "command": "expand_abbreviation_by_tab",

      // Extend Emmet to js & jsx
      "context": [
          {
            "operand": "source.js",
            "operator": "equal", 
            "match_all": true, 
            "key": "selector"
          },

          // run only if there's no selected text
          {
            "match_all": true, 
            "key": "selection_empty"
          },

          // don't work if completion popup is visible and you
          // want to insert completion with Tab. If you want to
          // expand Emmet with Tab even if popup is visible -- 
          // remove this section
          {
            "operand": false, 
            "operator": "equal", 
            "match_all": true, 
            "key": "auto_complete_visible"
          }
        ]
    },
    {"keys":["ctrl+q"],"command":"format_javascript"}
]
```
