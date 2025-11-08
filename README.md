# Consulting Document Builder

A collection of AI-powered bots designed to streamline the creation and editing of key business documents for consulting engagements.

## Project Overview

This project provides a series of specialized bots, run through BoodleBox, to automate and assist with the generation of proposals, reports, statements of work, and other common consulting documents. By leveraging these bots, you can ensure consistency, accuracy, and efficiency in your document workflow.

## Project Structure

This project is organized into a series of "Bot Sets," each contained in its own directory. The core of the project is the **Project Workflow Controller**, which acts as a central hub to guide the user to the correct specialized bot.

### `00_DocHelperSet`
- Contains the primary **Project Workflow Controller** (`00_DocHelper`).
- This controller's instructions include a `Specialized Bot Schema` that references the instruction files for all other bots.
- It manages the overall process but does not create document content itself.

### `01_CharterBuilderSet`
- Contains the specialized `PryorConsultingProjectCharterBuilder` bot.
- This bot is responsible for generating Project Charters.
- Its knowledge base, including the `CostStrategy.pdf` and `projectCharterTemplate.pdf`, is stored within this directory, making it a self-contained module.

This modular structure allows for easier maintenance and scalability. New bots can be added by creating a new `...Set` directory and updating the schema in the `00_DocHelper`.

## Usage

The workflow is initiated by interacting with the `@@PryorConsultingDocumentsHelper`. It will present a menu of options to guide you to the correct specialized bot based on your position in the project lifecycle.

For example, to start a new proposal, you would select the option that directs you to the `@@PryorConsultingProjectCharterBuilder`.

## Contributing

Contributions are welcome! If you'd like to improve the existing bots or add new ones, please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Commit your changes.
4.  Push your branch and submit a pull request.