## Html

Hyper Text Markup Language, é un linguaggio di Markup. Un linguaggio markup é un linguaggio di formattazione che segue determinate regole come l'impaginazione di un testo.

Un documento html é composto da tag annidati tra di loro.
Un tag si scrive aggiungendo al suo nome le parentesi angolari < nometag >

```
<nometag>

<element></element>

<padre>
  <figlio>
    <nipote>
       ...elementi annidati
    </nipote>
  </figlio>
</padre>
```

Sbagliato:

```
<padre>
  <figlio>
     <nipote>
  </figlio>
     </nipote>
</padre>
```

Corretto:

```
<padre>
  <figlio>
     <nipote>
     </nipote>
  </figlio>
</padre>
```

Difficile da capire per l'essere umano:

```
<padre><figlio><nipote></nipote></figlio></padre>
```

Difficile da capire per l'essere umano:

```
<padre>
<figlio>
<nipote>
</nipote>
</figlio>
</padre>
```

Semplice da capire:

```
<padre>
  <figlio>
    <nipote>
      <nipote></nipote>
    </nipote>
  </figlio>
  <iochisono>
    <nipote></nipote>
  </iochisono>
</padre>
```

### Attributi

Un tag può avere 1 o n attributi.

- Svolge una determinata funzione
- Chiave - Valore
- si scrive il nome dell'attributo
- si aggiunge uguale
- e tra apici si inserisce il valore

es.:
`nomeAttr="valore"`

`<element nomeAttr="valore"></element>`

sbagliato:
`<elementnomeAttr="valore"></element>`

sbagliato:
`<element nomeAttr=valore></element>`

sbagliato:
`<element nomeAttr="valore" nomeAttr="valore"></element>`

corretto:
`<element nomeAttr="valore" nomeAttr1="valore"></element>`

#### Attributi Globali

Un gruppo di attributi compatibili con tutti i tag html

#### Attributo ID

- É un attributo Globale
- accetta come valore una sola stringa di testo
- non bisogna utilizzare il carattere spazio nella stringa
- un'id deve essere univoco all'interno del documento
- ID serve ad identificare un solo elemento nel documento

es.: ` id="il-mio-id"`
es.: `<element id="il-mio-id"></element>`
es.: `<h1 id="il-mio-id"></h1>`

sbagliato:
`<element id="il-mio id"></element>`

sbagliato:
`<element id="il-mio prova"></element>`

corretto:
`<element id="il-mio-id"></element>`

trova l'errore:

```
<element id="hello"></element>
<element>
  <element>
    <element id="pippo">

    </element>
  </element id="pluto">
</element>
```

trova l'errore:

```
<element id="hello"></element>
<element>
  <element>
    <element id="hello">

    </element>
  </element>
</element>
```

corretto:

```
<element></element>
<element>
  <element>
    <element id="hello">

    </element>
  </element>
</element>
```

### Tag Html

[Lista completa di tutti i tag html](https://www.w3schools.com/tags/default.asp)
