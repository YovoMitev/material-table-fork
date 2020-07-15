## material-ui fork !!!
## original source
https://material-table.com/#/
## Needed feature

```jsx
                <MaterialTable
                  detailPanel={[
                    {
                      openedRows: [0, 1],
                       handleIconClick: (data) => console.log('FUCK MATERIAL TABLE', data),
                      render: data => <div>Fuck</div>
                    }
                  ]}
                  editable={{
                    // isDeletable: false,
                    disableCreateButton: true,
                    disableCancelButton: false,
                    // onRowAdd: () => console.log('ADD'),
                    onRowCancel: () => console.log('CANCEL'),
                    // onRowUpdate: () => console.log('ADD'),
                    // onRowDelete:() => console.log('ADD'),
                  }}
                />
```

```bash
detailPanel now you can pass openedRows as a array of IDS that will be always opened as a detail preview on each row
handleIconClick: function that will be trigger when click on detailPanel ICON
hideAllRows: function that will be trigger when page is change and will clear all visible detail panels
```