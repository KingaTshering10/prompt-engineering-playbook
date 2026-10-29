# Review notes

## What was prepared

This repository packages a prompt-engineering training collection. The supplied archive contains nine Word documents, one PDF, one Excel workbook, two copies of a JPEG image, one WAV audio file, and one MP4 video: **15 original files in total**.

The preparation adds a README, this inspection record, and Git exclusions. The original folder names, filenames, Office metadata, documents, workbook, and media are retained unchanged. macOS resource-fork files under `__MACOSX` are excluded.

## Content and inspection scope

- Text was extracted from all nine Word documents and the complete HR policy PDF to identify topics and document references.
- Office file packages were checked for archive integrity. Common embedded API-key and private-key signatures were not found in their XML content or the extracted document text. This pattern scan is not a comprehensive security guarantee.
- The workbook was opened read-only for inspection. It has one visible sheet, eight columns, and twelve campaign records. No cell formulas or external workbook links were found.
- Media metadata was inspected: the WAV is approximately 2.99 seconds, and the MP4 is approximately 114.17 seconds. The audio and video were not fully transcribed or reviewed for their spoken content.
- No prompts were submitted to an AI service. No outputs were generated, benchmarked, or validated against an answer key.
- Copy verification checks compare each original file with its corresponding bytes in the uploaded archive.

## Reference context

The HR PDF identifies The OpenGov Foundation and carries a last-updated date of 2018-01-08. The public upstream manual contains matching organization and date information:

https://github.com/opengovfoundation/hr-manual/blob/master/markdown/manual.md

It is an external reference for the chatbot exercise, not the maintainer's employment policy.

The finance exercises name Fabrikam, Adatum, Northwind Traders, and other training scenarios. The collection does not establish these files as real audited company records. Dates and derived metrics should be interpreted within the exercise rather than automatically updated to today's date.

## Example source-data inconsistency

In the Adatum financial-results document, the `N - 5` row lists revenue of 94,935 and cost of goods sold of 67,089, with a gross profit margin of 22.61%. The margin implied by those two amounts, `(revenue - cost of goods sold) / revenue`, is approximately **29.33%**. The preparation does not reconcile or overwrite the source figures.

Use this as an opportunity to verify assumptions and arithmetic when evaluating an AI-generated financial summary. The workbook and narrative documents should not be treated as an authoritative answer key for one another.

## Responsible AI examples

`M1/RAI.docx` intentionally includes requests about unsafe or inappropriate topics. It is retained as a set of response-evaluation examples, without adding instructions for carrying out the requests. An exercise can examine whether a tool sets appropriate boundaries, protects privacy, avoids unsupported claims, and redirects to a suitable alternative.

Some source exercises refer to tool interfaces, cloud services, or features that may change over time. No claim is made that every original step works with every account or current product version. The resource collection itself requires no programming runtime.

## Attribution

The archive does not include collection-wide licensing or complete attribution records for the documents and media. Original metadata is preserved and ownership is not reassigned. The repository's new overview is documentation of the supplied collection rather than a claim of original authorship of its training assets.
