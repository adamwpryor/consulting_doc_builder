# Consulting Document Builder

A collection of AI-powered bots designed to streamline the creation and editing of key business documents for consulting engagements.

## Project Overview

This project provides a series of specialized bots, run through BoodleBox, to automate and assist with the generation of proposals, reports, statements of work, and other common consulting documents. By leveraging these bots, you can ensure consistency, accuracy, and efficiency in your document workflow.

## Project Structure

This project is organized into a numeric series of bot directories. This numeric convention allows for logical grouping of bot types and the foundational models they run on. The core of the project is the **Project Workflow Controller** in directory `000`.

### `000` - Workflow Controller

- **Foundation Model:** Claude Sonnet 4.5
- Contains the primary **Project Workflow Controller** (`00_DocHelper`).
- This controller's instructions include a `Specialized Bot Schema` that references the instruction files for all other bots.
- It manages the overall process but does not create document content itself.

### `100` Series - Document Builders

- **Foundation Model:** GPT 4.1
- This series contains bots focused on document creation.
- **`101`**: Contains the `PryorConsultingProjectCharterBuilder` bot and all of its assets, including instruction files and knowledge base documents (`CostStrategy.pdf`, etc.).
- **`102`**: Contains the `PryorConsultingSOWBuilder` bot, which transforms an approved Project Charter into a final, binding Statement of Work.

### `200` Series - Meeting Analysis

- **Foundation Model:** Claude Opus 4.1
- This series contains bots focused on analyzing meeting notes and processing change requests.
- **`201`**: Contains the `PryorConsultingInitialMeetingSynthesizer` bot. This bot analyzes raw meeting notes or transcripts to extract key information and generate a structured synthesis and a JSON object for the Charter Builder.
- **`202`**: Contains the `ChangeRequestProcessor` bot. This bot analyzes client feedback from meeting notes against an existing document (like a Project Charter) to produce a Revision Impact Report and a JSON change log.

This modular structure allows for easier maintenance and scalability. New bots can be added by creating a new directory with the appropriate series number and updating the schema in the `000/00_DocHelper`.

## Usage

The workflow is initiated by interacting with the `@@PryorConsultingDocumentsHelper`. It will present a menu of options to guide you to the correct specialized bot based on your position in the project lifecycle.

For example, to start a new proposal, you would select the option that directs you to the `@@PryorConsultingProjectCharterBuilder`. To finalize an approved proposal into a contract, you would use the `@@PryorConsultingSOWBuilder`.

## Contributing

Contributions are welcome! If you'd like to improve the existing bots or add new ones, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes.
4. Push your branch and submit a pull request.
