```json
{
  // Place your snippets for typescriptreact here. Each snippet is defined under a snippet name and has a prefix, body and
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
  "Import styles": {
    "prefix": "csimpsty",
    "body": [
      "import styles from './index.css'",
      "",
      "const {",
      "  $1",
      "} = styles"
    ],
    "description": "Log output to console"
  },
  "Import Preact Styles Module": {
    "prefix": "csimppreacsty",
    "body": ["import styles from './index.module.scss'"],
    "description": "Log output to console"
  },
  "React Component with CSS Handles": {
    "prefix": "cscompcsshandles",
    "body": [
      "import React from 'react'",
      "import type { FC } from 'react'",
      "import { useCssHandles } from 'vtex.css-handles'",
      "import type { CssHandlesTypes } from 'vtex.css-handles'",
      "import './index.css'",
      "",
      "const CSS_HANDLES = [",
      "  ${2:Classes}",
      "] as const",
      "",
      "type ${1:${TM_FILENAME_BASE}}Props = {",
      "  classes?: CssHandlesTypes.CustomClasses<typeof CSS_HANDLES>",
      "}",
      "",
      "const ${1:${TM_FILENAME_BASE}}: FC<${1:${TM_FILENAME_BASE}}Props> = ({ classes }) => {",
      "  const { handles } = useCssHandles(CSS_HANDLES, { classes })",
      "",
      "  return <div className={handles.${3:Conatiner class}}>${1:${TM_FILENAME_BASE}}</div>",
      "}",
      "",
      "export default ${1:${TM_FILENAME_BASE}}"
    ],
    "description": "React component with css handles implementation"
  },
  "Export by default": {
    "prefix": "csexportdef",
    "body": [
      "export { default } from './src/components/${1:${TM_FILENAME_BASE}}'"
    ],
    "description": "React component with css handles implementation"
  },
  "Import and export before default": {
    "prefix": "csimporexportdef",
    "body": [
      "import { ${1:${TM_FILENAME_BASE}} } from './src/components/${2:Dir}'",
      "export default ${1:${TM_FILENAME_BASE}}"
    ],
    "description": "React component with css handles implementation"
  },
  "React Provider": {
    "prefix": "cscomprovider",
    "body": [
      "import React, { createContext, ReactNode, useContext, useMemo } from 'react'",
      "",
      "export interface ${1:${TM_FILENAME_BASE}}Type {}",
      "",
      "const ${1:${TM_FILENAME_BASE}} = createContext<${1:${TM_FILENAME_BASE}}Type>({} as ${1:${TM_FILENAME_BASE}}Type)",
      "",
      "export const use${1:${TM_FILENAME_BASE}} = () => useContext(${1:${TM_FILENAME_BASE}})",
      "",
      "export const ${2:Component}Provider = ({",
      "  children,",
      "}: {",
      "  children: ReactNode",
      "}) => {",
      "  const context = useMemo(() => {",
      "    return {}",
      "  }, [])",
      "",
      "  return <${1:${TM_FILENAME_BASE}}.Provider value={context}>{children}</${1:${TM_FILENAME_BASE}}.Provider>",
      "}",
      ""
    ]
  },
  "Preact Provider": {
    "prefix": "cspreactcomprovider",
    "body": [
      "import preact, { createContext, FunctionalComponent } from 'preact';",
      "import { useContext, useMemo } from 'preact/hooks';",
      "",
      "export interface ${1:${TM_FILENAME_BASE}}Type {}",
      "",
      "const ${1:${TM_FILENAME_BASE}} = createContext<${1:${TM_FILENAME_BASE}}Type>({ } as ${1:${TM_FILENAME_BASE}}Type)",
      "",
      "export const use${1:${TM_FILENAME_BASE}} = () => useContext(${1:${TM_FILENAME_BASE}})",
      "",
      "export const ${2:Component}Provider: FunctionalComponent = ({ children }) => {",
      "  const context = useMemo(() => {",
      "    return {}",
      "  }, [])",
      "",
      "  return <${1:${TM_FILENAME_BASE}}.Provider value={context}>{children}</${1:${TM_FILENAME_BASE}}.Provider>",
      "}",
      ""
    ]
  },
  "Preact Component": {
    "prefix": "cspreactcomponent",
    "body": [
      "import preact from 'preact';",
      "import styles from './index.module.scss';",
      "",
      "export const ${1:${TM_FILENAME_BASE}} = () => {",
      "  return <div className={styles.container}>${1:${TM_FILENAME_BASE}}</div>;",
      "};"
    ]
  }
}
```
