## jQuery Inline Affirm

jQuery Inline Affirm gives you an inline call to action and confirmation without having to mess with dialogs. It includes 3 styles: button, dark and light but can be styled easily.

demo: http://ashcraig.com/jq-inline-affirm/

## How to use

html : create a div element with the class "affirm" and style with "light", "dark" or "button" classes

EXAMPLE 

<code><div class="affirm button" data-id="1111" data-title="Save" data-question="Save this document?"></div></code>

- data-id : a unique id for the created element
- data-title : the title of the affirm link
- data-question : the question to affirm
- data-result : optional : text or html to display once affirmed

jQuery :

$(".affirm").inlineAffirm({
	callback : function(ele){
		console.log( $(ele).attr("data-id" ));
	}
});


