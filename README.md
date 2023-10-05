# Reproduction of Parcel issue #9296

See: https://github.com/parcel-bundler/parcel/issues/9296

## Steps to reproduce the issue

1. Run: npm install
2. Run: npm start
3. Check that watching start correctly.
4. Change the main.css content and see that the watcher works.
5. Add a typo in the class inside stories/my-story/my-component.css like this "bg-red-500" --> "bg-reed-500".
6. See an error is shown in the terminal.
7. Fix the previous typo.
8. See that watcher doesn't trigger a new rebuild.
9. Change main.css content.
10. See that now the watcher triggers rebuild normally.
