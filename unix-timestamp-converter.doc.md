# unix-timestamp-converter

Convert Unix timestamps into human-readable dates with automatic unit detection.

- Input: integer timestamp (seconds, milliseconds, microseconds, or nanoseconds).
- Output: ISO 8601 UTC string with trailing Z, readable local date, and unit details.
- Controls: copy ISO string, use current time shortcut, and clear/reset.
- Notes: sub-second precision is preserved in the ISO fractional portion when provided.
