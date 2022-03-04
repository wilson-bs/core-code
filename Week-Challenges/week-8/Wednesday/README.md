## Answers Wednesday 02/03/2022
### 1 - Create some links to various search engines.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Challenge 1 - Wednesday</title>
</head>
<body>
    <h1>Search Engines</h1>

    <ul>
        <li> <a href="https://www.google.com/">Google</a> </li>
        <li> <a href="https://www.bing.com/">Bing</a> </li>
        <li> <a href="https://search.yahoo.com/">Yahoo!</a> </li>
    </ul>
</body>
</html>
```

### 2 - Display five different images. Each image should have a title.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Challenge 2 - Wednesday</title>
</head>
<body style="color: rgb(48, 0, 34);">
    <h1>Display five different images | Dogs</h1>
    <table border="2" style="background-color: rgb(134, 196, 255);">
		<tr>
			<th>Labrador</th>
			<th>Golden</th>
			<th>Pitbull</th>
			<th>Corgi</th>
            <th>Dogo de Burdeos</th>
		</tr>
		<tr>
			<td>
				<img src="https://images.unsplash.com/photo-1518717758536-85ae29035b6d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" title="Labrador" height="100px">
			</td>
			<td>
				<img src="https://images.unsplash.com/photo-1536809188428-e8ecf663d0be?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" title="Golden" height="100px">
			</td>
			<td>
				<img src="https://images.unsplash.com/photo-1477884213360-7e9d7dcc1e48?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" title="Pitbull" height="100px">
			</td>
			<td>
				<img src="https://images.unsplash.com/photo-1600077106724-946750eeaf3c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" title="Corgi" height="100px">
			</td>
            <td>
				<img src="https://images.unsplash.com/photo-1541599540903-216a46ca1dc0?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=871&q=80" title="Dogo de Burdeos" height="100px">
			</td>
		</tr>
	</table>
</body>
</html>
```

### 3 - Display an image that when clicked will link to a website of your choice (should be opened in a new window).
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Challenge 3 - Wednesday</title>
</head>
<body style="color: rgb(48, 0, 34);">
    <h1>Image that when clicked will link to a website</h1>
   
    <table border="2" style="background-color: rgb(134, 196, 255);">
		<tr>
			<th>CoreCode</th>

		</tr>
		<tr>
			<td>
                <a href="https://www.core-code.io/" target="_blank" title="link">
                    <img src="https://uploads-ssl.webflow.com/5eb2f56932c3562feab232e3/5f73550d00249e7e96c9f3de_Logo.png" title="Link to CoreCode" height="100px">
                </a>
			</td>
			
		</tr>
	</table>
</body>
</html>
```