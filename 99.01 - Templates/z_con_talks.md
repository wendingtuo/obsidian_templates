___
**Date**: *[[<% tp.date.now("YYYY-MM-DD") %>]]*
**Time**: *<% tp.date.now("HH:mm") %>*
**MOC**: 
**People**: 
**Tags**: 
___
<%*
	let title = tp.file.title
	if (title.startsWith("Untitled")) {
    let title = await tp.system.prompt("Title")
    let date = tp.date.now("YYYY-MM-DD HH.mm")
	await tp.file.rename(`${date}` + ' - ' + `${title}`);
	}
%>
## Links:

- 

## Notes: 

- 

