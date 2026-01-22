# Party Component Task (Module 0) -> Moqui


## Project Structure

- `component.xml` — Moqui component descriptor
- `MoquiConf.xml` — Moqui configuration for this component
- `data/`
  - `PartyDemoData.xml` — Demo data for parties
  - `PartyEnumData.xml` — Enumeration data for party types, roles, etc.
- `entity/`
  - `Entities.xml` — Entity definitions (Person, Party, etc.)
- `screen/`
  - `PartyScreen.xml` — Screen definitions for party management UI
- `script/`
  - `CreatePersonScript.groovy` — Groovy script for creating a person
- `service/`
  - `person.rest.xml` — REST service definitions
  - `PersonServices.xml` — Service definitions for party operations

## Getting Started

### Prerequisites
- [Moqui Framework](https://www.moqui.org/)
- Java 8 or higher

### Setup

### Development Flow

I started this project by designing the core structure and creating the necessary folders step by step:

1. **entity/**: Defined all the main entities (such as Person, Party, etc.) in `Entities.xml` to establish the data model.
2. **data/**: Added `PartyEnumData.xml` for enumeration values and `PartyDemoData.xml` for demo records to support development and testing.
3. **service/**: Implemented business logic and REST APIs in `PersonServices.xml` and `person.rest.xml` to handle party operations.
4. **screen/**: Built the user interface screens in `PartyScreen.xml` for managing parties through the Moqui UI.
5. **script/**: Wrote utility scripts like `CreatePersonScript.groovy` to automate and demonstrate key operations.
6. Created `component.xml` and `MoquiConf.xml` to register the component and configure it within the Moqui framework.

This folder-by-folder approach ensured a modular, organized, and scalable development process.

### Loading Demo Data
Demo and enum data are loaded automatically if referenced in `component.xml`.

## Features
- Party (Person/Organization) entity definitions
- Demo and enum data for quick setup
- REST and service layer for party operations
- UI screens for party management
- Example Groovy script for person creation
