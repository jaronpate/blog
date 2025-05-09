The lexer.

<terminal :rows="1" :lines="[
    'yarn add chevrotain'
]"></terminal>

```javascript
export class Parser extends chevrotain.CstParser {

    constructor() {
        super(allTokens);

        const $ = this;

        $.RULE('concatFunction', () => {
            $.CONSUME(ConcatFunc);
            $.CONSUME(OpenParen);
            $.MANY_SEP({
                SEP: Comma,
                DEF: () => {
                    $.SUBRULE($.expression, { LABEL: 'value' });
                }
            });
            $.CONSUME(CloseParen);
        });
    }
}
```