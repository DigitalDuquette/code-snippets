# Azure Data Studio Code Snippets

Code snippets in Azure Data Studio: repetition is no guarantee for memorization.

![syntax-emotions](miscellany/img/what_was_that_syntax.png)

ADS snips are a core part of developing with t-sql and I use this batch of snippets daily.

## Install your snippets

To update your code snippets, open the command pallet and paste in the contents of the .json file in this repo.

![how to install](miscellany/install-snippet.gif)

Local (macOS) file repository:
> /Users/digitalduquette/Library/Application Support/azuredatastudio/User/snippets/sql.json

For more information on code-snippets visit the [blog article](https://docs.microsoft.com/en-us/sql/azure-data-studio/code-snippets?view=sql-server-2017).

## Formatting

Place your global snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope is left empty or omitted, the snippet gets applied to all languages. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are: $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders.

Placeholders with the same ids are connected.

**Example**:
```json
"Print to console": {
"scope": "javascript,typescript",
"prefix": "log",
"body": [
		"console.log('$1');",
		"$2"
	],
	"description": "Log output to console"
}
```
