## Copy Trello board script

This script copies a Trello board and replaces the references on the new board's cards' checklists with references to cards.

:warning: Linux users need to install Swift on their machines. If this turns out as not possible, these are the available options:
1. Ask someone with MacOS to run this script for you (reach out to @dtilve).
2. Copy the board yourself and restore the links manually.

Coded in Swift 3.2 using [Marathon](https://github.com/JohnSundell/Marathon)

### Requisites
Marathon:
- [Marathon Requirements](https://github.com/JohnSundell/Marathon#requirements)
- [Marathon Installation](https://github.com/JohnSundell/Marathon#installing)

### Usage

This script expects 4 arguments passed as literal strings in `argv` in the following order:
1. API key
2. Token
3. Board ID (this is the 8 character long path in the board's URL)
4. New board name

Install marathon and run as:
`$ marathon run copyTrello "API_KEY" "TOKEN" "BOARD_ID" "NEW_BOARD_NAME"`
