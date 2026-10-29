# Prompt Engineering Playbook

### Practical exercises for writing, refining, and evaluating AI prompts

![Focus](https://img.shields.io/badge/Focus-Prompt_Engineering-2563EB)
![Learning](https://img.shields.io/badge/Format-Hands--on_Exercises-059669)
![Topics](https://img.shields.io/badge/Topics-Copilot_%7C_Multimodal_AI_%7C_Finance-7C3AED)

A collection of prompt-engineering training materials covering content creation, document-based Q&A, responsible AI, enterprise scenarios, financial analysis, and multimodal examples. It brings together exercise documents and the reference files needed to try them.

The original materials are retained in their supplied folders. This is a **learning-resource repository**: it contains documents, a spreadsheet, images, audio, and video rather than an application to install or run.

**[Start here](#start-here) · [Learning path](#suggested-learning-path) · [Resource guide](#resource-guide) · [Practice method](#a-simple-practice-method) · [Source notes](#source-notes)**

## What the collection covers

- Writing prompts with a clear task, context, constraints, tone, and output format.
- Refining drafts through follow-up instructions.
- Creating content, extracting information, and requesting structured outputs.
- Answering questions from an attached reference document.
- Exploring responsible AI boundaries and evaluating responses.
- Working through enterprise IT and finance scenarios.
- Using image, audio, and video examples in tools that support those inputs.

## Start here

1. Download the repository ZIP, or clone it:

   ```bash
   git clone https://github.com/KingaTshering10/prompt-engineering-playbook.git
   cd prompt-engineering-playbook
   ```

2. Open a Word exercise document and choose one task.
3. Open the AI tool used by that exercise and attach the referenced file when required.
4. Try the prompt, review the response, and refine one part at a time.

There is no Python environment, `requirements.txt`, or API integration in this repository. Use a compatible document reader, spreadsheet application, and media player to view the resources. Some exercises refer to Microsoft Copilot, Microsoft 365 apps, or Google AI Studio; available features and file support depend on the tool, account, and version you use.

## Suggested learning path

| Stage | Resources | Learning goal |
| --- | --- | --- |
| 1. Prompt basics | `M1/basic_copilot.docx` | Practice roles, context, constraints, tone, and structured responses |
| 2. Content creation | `M1/content creation.docx` | Adapt prompts for blogs, campaigns, and travel content |
| 3. Reference-based Q&A | `M1/chatbot/` | Ask questions grounded in an attached policy document |
| 4. Advanced scenarios | `M2/` | Explore few-shot examples, prompt structure, and enterprise problem analysis |
| 5. Finance workflows | `Finance/` | Work with tables, campaigns, reports, and financial summaries |
| 6. Multimodal practice | `4GoogleAIStudio/` | Explore image, audio, and video inputs |

Use `M1/RAI.docx` alongside these stages to discuss responsible AI behavior. It intentionally includes problematic requests as evaluation examples; the collection does not provide instructions for carrying out those requests.

## Resource guide

### Module 1 — Foundations

| File | Purpose |
| --- | --- |
| [Basic Copilot prompts](M1/basic_copilot.docx) | Writing, editing, role-based prompting, structured output, and information extraction exercises |
| [Content creation](M1/content%20creation.docx) | Example prompts for healthcare content, social media, and travel writing |
| [Responsible AI examples](M1/RAI.docx) | Discussion prompts covering safety, privacy, fairness, misuse, and reliability |
| [Street image](M1/street.jpg) | Image input for captioning and visual-description exercises |
| [Chatbot prompts](M1/chatbot/chatbot-prompts.docx) | Questions to ask about the accompanying reference PDF |
| [HR policy manual](M1/chatbot/HR%20policy%20manual.pdf) | Historical reference document for document-grounded Q&A |

The HR manual identifies **The OpenGov Foundation** and is dated **8 January 2018**. It is supplied as an exercise reference, not as the current policy of the repository maintainer or their employer. See the [upstream manual](https://github.com/opengovfoundation/hr-manual/blob/master/markdown/manual.md) for attribution and context.

### Module 2 — Advanced prompting

| File | Purpose |
| --- | --- |
| [Advanced Copilot prompts](M2/advanced-prompts_copilot.docx) | Separators, few-shot sentiment examples, image prompts, structured analysis, and document-conversion requests |
| [Enterprise modernization scenario](M2/IT_Scenario_Enterprise_Modernization.docx) | A Northwind Industrial Systems case study involving cloud performance, security, cost, and operational resilience |

The enterprise case is an exercise description. It does not include an implemented remediation, a deployed cloud environment, or verified operational results.

### Finance exercises

| File | Purpose |
| --- | --- |
| [Copilot finance use cases](Finance/usecase_copilot.docx) | Email drafting, campaign analysis, report writing, and financial-summary exercises |
| [Fabrikam campaign workbook](Finance/Fabrikam%20Q1%20marketing%20campaigns.xlsx) | Twelve campaign records for calculations, comparisons, and charting practice |
| [Fabrikam campaign reference](Finance/Fabrikam%20Q1%20marketing%20campaign%20data.docx) | Campaign figures and existing summaries for report-writing exercises |
| [Adatum financial results](Finance/Adatum%205%20Year%20Financial%20Results.docx) | Five periods of financial figures for analysis and summarization practice |

Treat the figures as supplied training inputs. Check arithmetic and metric definitions rather than assuming every existing summary is correct. The workbook contains one sheet with twelve campaign rows and no formulas. Some dates and derived values in the documents are historical snapshots; the Adatum periods use `N` as an unspecified current year. [Review notes](docs/review-notes.md) record an example of a source-data inconsistency without changing the originals.

### Multimodal assets

| File | Purpose |
| --- | --- |
| [Street image](4GoogleAIStudio/street.jpg) | Image input; the same image is also retained in `M1/` |
| [Audio sample](4GoogleAIStudio/time.wav) | Short WAV input, approximately three seconds long |
| [Video sample](4GoogleAIStudio/responsible_ai.mp4) | MP4 input, approximately one minute and fifty-four seconds long |

These are example assets, not a labeled benchmark. No transcripts, expected model responses, or measured performance results are provided.

## A simple practice method

For each exercise, record:

| Item | What to capture |
| --- | --- |
| Task | The result you want and its intended audience |
| Inputs | The document, image, or data used as context |
| Prompt | Your exact instructions and output format |
| Tool | Product and model/version information, when available |
| Review | Whether the response followed instructions and matched the source |
| Revision | One change to the prompt and what changed in the response |

For document Q&A, ask for the relevant section or page and verify it against the attachment. For calculations, compare the response with the source values and your own arithmetic. For reasoning tasks, request a concise explanation, explicit assumptions, and checkable recommendations.

Store your generated drafts and experiments under `practice-output/`, which is excluded from Git by default. Nothing in this repository automatically submits prompts, uploads attachments to an AI service, sends emails, or modifies cloud resources.

## Source notes

Prepared from the supplied training archive, preserving **15 original files byte for byte**. The collection includes third-party training content and reference assets; authorship and ownership are not assigned to the repository maintainer. Original document metadata remains intact. No collection-wide license was supplied, so this repository does not apply a new license to those materials.

Useful official references:

- [Google AI Studio quickstart](https://ai.google.dev/gemini-api/docs/ai-studio-quickstart)
- [Microsoft: Copilot Chat in Microsoft 365 apps](https://support.microsoft.com/en-us/microsoft-365-copilot/how-copilot-chat-works-in-microsoft-365-apps)
- [OpenGov Foundation HR manual](https://github.com/opengovfoundation/hr-manual)

See [review notes](docs/review-notes.md) for inspection scope and source limitations.

Maintained by **[Kinga Tshering](https://github.com/KingaTshering10)**.
