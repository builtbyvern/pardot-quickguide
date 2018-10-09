# Pardot Templates

## Email:

[https://help.salesforce.com/articleView?id=pardot_email_templates.htm&type=5]()

### Editable Content: `<div pardot-region></div>`

Can be any element (div, td, etc...). Using this tag makes the region editable within Pardot.

### Repeatable Content: `<div pardot-repeatable></div>`.

Repeatable content must have a pardot-region within it.

```html
<div pardot-repeatable>
    <table>
        <tr>
            <td pardot-region>
                Editable Content
            </td>
        </tr>
    </table>
</div>
```

### Removable Content: `<div pardot-removable=”Name of the section”></div>`

Must also contain a pardot-region like above.


## LP’s

I’d recommend [this guide](https://www.pardot.com/training/creating-layout-templates/).

[Wanna go crazy with forms?](https://help.salesforce.com/articleView?id=pardot_forms_layout_template_form_code.htm&type=5)

### Editable Content

Uses `pardot-region` like the emails. This seems to be the only pardot tag for the user-side. 

```html
<div pardot-region=”Sidebar”>
    <h3>More Links</h3>
</div>
```

Pairs well with `pardot-region-type` (link, image, html, simple, and wysiwyg). Defaults to wysiwyg. 

```html
<a href="https://jennamolby.com" pardot-region="editable-link" pardot-region-type="link">My Link</a>

<img src="image/my-image.png" pardot-region="editable-image" pardot-region-type="image" />

<code pardot-region=”pardot_html” pardot-region-type=”html”><here is some code></code> 

<p pardot-region="simple-text" pardot-region-type="simple">Your text here.</p>

```
### Snippets

- [https://jennamolby.com/a-collection-of-incredibly-useful-pardot-snippets/]()
- [https://marcloudconsulting.com/development/pardot-content-regions-101]()







