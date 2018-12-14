# angular-autocomplete
Autocomplete component for Angular

### Call this component (HTML):
```
<app-autocomplete
  [data]="autocompleteData"
  [update]="autocompleteUpdate"
  (onItemSelected)="itemSelected($event)">
</app-autocomplete>
```

### Declare data values (Javascript/Typescript):

```
public autocompleteData: AutocompleteObject;
public autocompleteUpdate = new EventEmitter<AutocompleteObject>();
```

```
this.autocompleteData = {
  placeholder: 'Search for items',
  minCharacters: 0,
  maxResults: 0,
  cleanInputOnSelection: true,
  items: ['Pizza', 'Burger', 'Kebab']
};
this.autocompleteUpdate.emit(this.autocompleteData);
```
