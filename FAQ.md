# Frequently Asked Questions (FAQ)

### Do I still need the workflow with recent versions of Google Drive?

Since the Google Drive app switched to the macOS File Provider API, you may no longer need a workflow as Google Drive files may show up in regular Alfred searches. If you’re not seeing them, go into Alfred Preferences → Features → Default Results → Search Scope → Reset… (bottom right) and `Reset to Applications and Home`. This may not work for everyone, it depends on the underlying macOS index.

### Can I keep running the workflow anyway?

Yes. Some people still prefer it for its granularity and features.

### How do I report an issue?

Accurate and thorough information is crucial for a proper diagnosis. **At a minimum, your report should include:**

* The output of running `!gddiagnostic`.
* The [debugger](https://www.alfredapp.com/help/workflows/advanced/debugger/) output of the failing action.
