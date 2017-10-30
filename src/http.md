# Go Http


## HTTP Request with Custom Header

```go
client := &http.Client{}
req, err := http.NewRequest("GET", "http://example.com", nil)
req.Header.Add("If-None-Match", `some value`)
resp, err := client.Do(req)
```
