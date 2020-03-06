document.addEventListener("DOMContentLoaded", function(e) {
	document.cookie = "accessToken=efjkqr3kl34rkbgruiq34o7qelfu4phqofaf;max-age=" + 60*60;
	document.cookie = "floof=1234;max-age=" + 60*60;
	let cookies = {};
	document.cookie.split("; ").forEach(cookie => {
		cookies[cookie.split("=")[0]] = cookie.split("=")[1];
	});
	console.log(cookies);
	fetch("http://localhost:4000/blogs", {
		method: "POST",
		headers: {
			"Content-Type": "application/x-www-form-urlencoded",
			"Authorization": `Bearer ${cookies.accessToken}`
		},
		body: "title=Feta&content=Feta er godt, meget feta er meget godt."
	});
});