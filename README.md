# Ai Incrementor

Simple JS script to auto-increment values in an Illustrator document.

# CREDITS
 
You are free to use, modify, and distribute this script as you see fit. No credit is required but would be greatly appreciated. 

Scott Lewis
* scott@atomiclotus.net
* https://atomiclotus.net

# DISCLAIMER OF LIABILITY

THIS SCRIPT IS OFFERED AS-IS WITHOUT ANY WARRANTY OR GUARANTEES OF ANY KIND. YOU USE THIS SCRIPT COMPLETELY AT YOUR OWN RISK AND UNDER NO CIRCUMSTANCES WILL THE DEVELOPER AND/OR DISTRIBUTOR OF THIS SCRIPT BE HELD LIABLE FOR DAMAGES OF ANY KIND INCLUDING LOSS OF DATA OR DAMAGE TO HARDWARE OR SOFTWARE. IF YOU DO NOT AGREE TO THESE TERMS, DO NOT USE THIS SCRIPT.

## Installation

1. Place the ai-incrementor.jsx script in Applications > Adobe Illustrator > Presets > en_US > Scripts
2. Restart Adobe Illustrator to activate the scripts
3. The script will be available under menu File > Scripts > Ai Incrementor
4. Select File > Scripts > Ai Incrementor
5. A new dialog will open with a list of all saved sessions (if you have any) and three buttons: Close, Open, Save. Select a saved session from the list, or double-click the name of the session to open it. Or, click "Save" to save the current session.
6. Sessions are saved in ~/ai-sessions/ai-YYYY-MM-DD-r[0-9].json
7. Errors are saved in ~/ai-sessions/ai-log-YYYY-MM-DD-r[0-9].txt

## Usage

You can add an auto-incrementing "counter" anywhere in your Illustrator document as long as you follow these instructions *exactly*. The script uses a "replacement token" to indicate where the counter should go. The token is `${#}` (dollar sign + left curly bracket + pound sign + right curly bracket).

The counter will replace the token with the next number in the iteration in the order in which the items were added (based on the layer order).

For now, this is a dead-simple implementation. In a future version I will add the ability to add multiple, independent counters as well as the ability to place counters anywhere in the document and in any text.

1. Add the `${#}` token to your document in a separate text frame (text object).
2. The `${#}` token should be the *only* thing in the text frame.
3. Go to _File > Scripts > Ai Incrementor_ and watch the magic. (It is super fast).
4. You can simply do _Undo_ to revert back to the `${#}` tokens if you need to change something.