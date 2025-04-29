### Question
- How semantically related are reviews to a perfume's listed notes?

### Approach 
1. Use `e5-large-instruct` to embed "high quality" reviews
2. Establish that semantic relatedness exists between review-embeddings and notes-embeddings by scoring reviews
  - e.g. a review that mentions every fragrance-note would score highest
3. Train a MLP to attempt to learn mappings between reviews and fragrance-notes

### Outcome
- `e5-large-instruct` doesn't think fragrantica.com reviews discuss fragrance notes very much at all!