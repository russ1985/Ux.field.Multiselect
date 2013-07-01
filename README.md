Ux.field.Multiselect
====================

Multiselect field for Sencha Touch 2.1/2.2 Works as a single or multi select field.

It can easily extend Ext.field.Text if to take the missing code from Ext.field.Select and add it to Ux.field.Multiselect.

usePicker config won't work as it is always used a list on both tablets and phones

Usage
```javascript
Ext.create('Ext.form.Panel', {
    fullscreen: true,
    items: [
        {
            xtype: 'fieldset',
            title: 'Select',
            items: [
                {
                    xtype: 'multiselectfield',
                    label: 'Choose one',
                    delimiter: ',', 
                    mode: 'SINGLE', // default is MULTI,
                    // value: ['first','second'] , init value with an array
                    // value: 'first,second', init value with a string
                    options: [
                        {text: 'First Option',  value: 'first'},
                        {text: 'Second Option', value: 'second'},
                        {text: 'Third Option',  value: 'third'}
                    ]
                }
            ]
        }
    ]
});
```

![Multiselect field](screenshot.png)

DEMO: https://rawgithub.com/vadimpopa/Ux.field.Multiselect/master/index.html

p.s For chrome users when testing, in the address bar at the right end should be a 'shield' icon, you can click on that to run insecure content. Those scripts are from http://cdn.sencha.io/touch/sencha-touch-2.2.0, don't worry it's safe.
 