### Recording Reliability

- Improved recording uploads so temporary backend, storage, transcription, or database failures return clear retryable errors instead of blank server errors.
- Hardened device session refresh so transient database lookups no longer look like upload failures.

### Diagnostics & Stability

- Reduced noisy Sentry reports from expected dictation finish disconnects and automatic network failure capture.
- Improved diagnostic tagging so recording, transcription, and dictation failures are easier to group.
- Moved microphone startup device selection off the main thread to reduce launch and capture stalls.
