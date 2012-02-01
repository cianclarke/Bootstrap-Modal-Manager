#Bootstrap Modal manager  
  
Allows creation of Bootstrap modal dialogs with optional params  
  
##Usage  
   
@param t : title string  
@param m : message string or HTML  
@param b : array of buttons, like [{text: 'Cancel'}, {text: 'Save', type: 'primary'}]  
where type is one of primary, info, success, danger  
@param opts: object of options from boostrap modal, namedly backdrop and keyboard  
  
    An example with a close button, no backdrop and no keyboard controls:
    var buttons = [
       {
         text: 'Save'
       },
       {
         text: 'Close'
       }
    ];
    modal("My Modal Dialog", "My Modal Message", buttons, { backdrop: false, keyboard: false });

