```json
{
  // Place your snippets for typescript here. Each snippet is defined under a snippet name and has a prefix, body and
  // description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
  // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the
  // same ids are connected.
  // Example:
  // "Print to console": {
  // 	"prefix": "log",
  // 	"body": [
  // 		"console.log('$1');",
  // 		"$2"
  // 	],
  // 	"description": "Log output to console"
  // }
  "React Basic Hook": {
    "prefix": "csreacthook",
    "body": [
      "import { useState, useEffect } from 'react'",
      "",
      "export interface ${1:${TM_FILENAME_BASE}}Type {}",
      "",
      "export const ${1:${TM_FILENAME_BASE}} = () => {",
      "  const [state, setState] = useState<${1:${TM_FILENAME_BASE}}Type>({})",
      "",
      "  useEffect(() => {",
      "    // Your code here",
      "  },",
      "  [])",
      "",
      "  return [state, setState]",
      "}",
      ""
    ]
  },
  "Preact Basic Hook": {
    "prefix": "cspreacthook",
    "body": [
      "import { useState, useEffect } from 'preact/hooks'",
      "",
      "export interface ${1:${TM_FILENAME_BASE}}Type {}",
      "",
      "export const ${1:${TM_FILENAME_BASE}} = () => {",
      "  const [state, setState] = useState<${1:${TM_FILENAME_BASE}}Type>({})",
      "",
      "  useEffect(() => {",
      "    // Your code here",
      "  },",
      "  [])",
      "",
      "  return [state, setState]",
      "}",
      ""
    ]
  }
}
```