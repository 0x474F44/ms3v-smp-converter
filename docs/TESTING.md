# Testing and bulk-conversion notes

1. Back up the original SD card.
2. Start with one or two files.
3. Then test a larger folder.
4. The converter processes files sequentially rather than all at once.
5. If one file fails, the converter records the error and continues.
6. Use **Copy Activity Log** to copy the full diagnostic log.

Common per-file failures can be caused by browser decoding limitations, corrupted media, unsupported codecs, or very large/problematic files. The converter does not discard the source file.

