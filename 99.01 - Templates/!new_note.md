<% tp.web.daily_quote() %>
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
    let date = tp.date.now("YYYY-MM-DD")
	await tp.file.rename(`${date}` + ' - ' + `${title}`);
	}
%>
## Notes: 

- 

