```mermaid
graph TD
    A[User writes a new note in the text field] --> B[User clicks Save button]
    B -->C[The browser sends a POST request to the server]
    C -->D[Server receives the request and processes the new note]
    D -->E[Server saves the note in the database]
    E -->F[Server responds with the new saved note]
    F -->G[The browser receives the response from the server]
    G -->H[Browser refreshes list of notes on page]

    
    C "POST Request"--> D
    F "Response with the new note" --> G
```