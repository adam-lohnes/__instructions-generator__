# Project Instructions Generator

A meta-project for generating comprehensive instructions for all future projects using Cursor AI.

## Purpose

This project provides a framework for creating detailed, structured instructions for any type of project, whether technical, creative, business, or personal. It helps to:

- Systematically plan new projects from inception to completion
- Create living documentation that evolves with the project
- Establish consistent workflows for development and tracking
- Leverage AI assistance effectively throughout the project lifecycle

## Structure

The project is organized as follows:

```
.cursor/rules/                     # Main Cursor rules
├── project_instruction_generator.mdc  # Rule for generating project instructions
├── cursor_rule_creator.mdc            # Rule for creating new Cursor rules
└── [other_rules].mdc                  # Additional specialized rules

project_templates/                 # Template examples for different project types
├── technical/
│   ├── web/
│   ├── mobile/
│   ├── api/
│   ├── data/
│   ├── game/
│   └── tool/
├── creative/
│   ├── writing/
│   ├── design/
│   └── media/
├── business/
│   ├── planning/
│   ├── marketing/
│   └── analytics/
└── personal/
    ├── life/
    ├── learning/
    └── productivity/
```

## Usage

1. Create a new empty project folder
2. Copy the appropriate rule from `.cursor/rules/` to your project
3. Use Cursor AI to generate detailed project instructions based on the rule
4. Follow the generated instructions to build your project systematically

## Core Rules

### Project Instruction Generator

This rule helps create comprehensive project plans and instructions tailored to your specific project needs. It guides you through:

- Initial project assessment and planning
- Creating structured project documentation
- Setting up appropriate tools and environments
- Establishing consistent workflows
- Tracking progress with journal entries
- Quality control and delivery processes

### Cursor Rule Creator

This rule helps you create new Cursor rules for specialized project types. It provides guidance on:

- Rule purpose and structure
- Development workflow for rules
- Organization and maintenance
- Best practices for effective rules

## Creating New Rules

To create a new specialized rule:

1. Start with a markdown (`.md`) file in the workspace root
2. Develop and refine the content
3. Test the rule by reviewing its effectiveness
4. Use the terminal to convert to a `.mdc` file and place in `.cursor/rules/`:
   ```bash
   cp your_rule.md .cursor/rules/your_rule.mdc
   ```
5. **IMPORTANT**: Place all rules directly in the `.cursor/rules/` directory without subdirectories
6. Use clear, descriptive filenames, with prefixes if helpful (e.g., `tech_web_app.mdc`)

## Extending This Project

To add support for new project types:

1. Use the Cursor Rule Creator to develop a new rule
2. Create example templates in the corresponding `project_templates/` directory
3. Remember that template organization can use subdirectories, but Cursor rules must all be placed directly in the `.cursor/rules/` directory 