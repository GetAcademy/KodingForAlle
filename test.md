```js
{
    rom: [
        { navn: 'A', innhold: ['rød nøkkel'], start: true },
        { navn: 'B', innhold: ['grønn nøkkel'] },
        { navn: 'C', innhold: ['hvit nøkkel'] },
        { navn: 'D', innhold: ['blå nøkkel'] },
        { navn: 'E', innhold: ['grå nøkkel'] },
        { navn: 'F', innhold: [], vunnet: true },
    ],
    dører: [
        { A: 'B', B: 'A', farge: 'rød', åpen: false },
        { A: 'D', D: 'A', farge: 'grønn', åpen: false },
        { B: 'C', C: 'B', farge: 'grå', åpen: false },
        { B: 'E', E: 'B', farge: 'blå', åpen: false },
        { E: 'F', F: 'E', farge: 'hvit', åpen: false },
    ]
};

```
