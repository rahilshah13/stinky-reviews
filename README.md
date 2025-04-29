How semantically related are reviews to a perfume's listed notes?

### Approach 
1. Use `e5-large-instruct` to embed "high quality" reviews

2. Score 'review' embeddings against 'notes' embeddings to establish that a semantic relatedness exists. A review that mentions every note in the fragrance scores highest.

3. Train a MLP to attempt to learn mappings between reviews and fragrance-notes

### Misc
- The full dataset is too large to push to github, but the notebook cells marked with checkpoint can be run

### Outcome
- `e5-large-instruct` doesn't think fragrantica.com reviews discuss fragrance notes very much at all!