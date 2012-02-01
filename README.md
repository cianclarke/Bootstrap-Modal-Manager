#Bootstrap Modal manager  
Allows creation of Bootstrap modal dialogs with optional params  
  
@param t : title string  
@param m : message string or HTML  
@param b : array of buttons, like [{text: 'Cancel'}, {text: 'Save', type: 'primary', callback: function(){}}]  
where type is one of primary, info, success, danger  
@param opts: object of options from boostrap modal, namedly backdrop and keyboard  
  
##Usage  
  
    // An example with a close button, no backdrop and no keyboard controls:
    var buttons = [
     {
       text: 'Save',
       type: 'primary'
     },
     {
       text: 'Close',
       callback: function(){
         // This is an ID appended onto all popups we make. This call will hide the window & remove it.
         $('#_modalGen').modal('hide');
         $('.modal').remove();
       }
     }
    ];
    modal("My Modal Dialog", "My Modal Message", buttons, { backdrop: false, keyboard: false });
