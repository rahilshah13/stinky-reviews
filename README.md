Do fragrance reviews on fragrantica.com mention notes?

### Approach 
1. Use `e5-large-instruct` to embed "high quality" reviews
2. Score review-embeddings against notes-embeddings per fragrance to verify relatedness. A review that mentions every note in the fragrance scores highest.
3. Use a MLP to attempt to learn mappings from reviews to fragrance-notes

### Misc
- The full dataset is too large to push to github, but the notebook cells marked with checkpoint can be run
- TODO: Test embedding invariance vs. input length (directional invariance)

### Outcome
- `e5-large-instruct` embeddings are viable for ranking reviews
- The MLP did not yield results
