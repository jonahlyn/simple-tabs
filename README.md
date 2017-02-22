# &lt;simple-tabs&gt;

&lt;simple-tabs&gt; is a custom polymer element to display content in a simple tabbed interface.



## Dependencies

Include the polyfill.

```
<script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
```

Import the component.

```
<link rel="import" href="simple-tabs.html">
```



## API

### &lt;simple-tabs&gt;

Section elements are used to deliniate the content for the different tabs.

```
<simple-tabs>
    <section>
        <h2>First</h2>
        <p>Section 1 content.</p>
    </section>
    <section>
        <h2>Second</h2>
        <p>Section 2 content.</p>
    </section>
    <section>
        <h2>Third</h2>
        <p>Section 3 content.</p>
    </section>
</simple-tabs>
```



### Selected Attribute

The first section element will be the default selected tab.
You can change the default tab by adding a `selected` attribute to another section.
In the example below, the third tab will be the default.

```
<simple-tabs>
    <section>
        <h2>First</h2>
        <p>Section 1 content.</p>
    </section>
    <section>
        <h2>Second</h2>
        <p>Section 2 content.</p>
    </section>
    <section selected>
        <h2>Third</h2>
        <p>This is the new default tab.</p>
    </section>
</simple-tabs>
```

You can also change the selected tab programatically as follows:

```
let e = document.querySelector('simple-tabs');
e.selectTab(document.querySelector('#tab-2'));
```


### Tab Titles

The first heading in any section will become the tab title text.
Titles can be set by using the `title` attribute.
The default text is simply 'Tab'.

```
<simple-tabs>
    <section>
        <h2>First</h2>
        <p>Section 1 content.</p>
    </section>
    <section title="Section 2">
        <h2>Second</h2>
        <p>Section 2 content.</p>
    </section>
    <section>
        <p>This section has no title.</p>
    </section>
</simple-tabs>
```

## License

TBD