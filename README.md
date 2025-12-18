# CS Diagrams

A collection of computer science diagrams, database schemas, and technical documentation.

## Contents

- **[Discount Tire ERD](discount_tire_erd.md)** - Entity Relationship Diagram for a Discount Tire service business
  - 23 tables covering customers, mechanics, garages, cars, tires, services, and financials
  - Complete service tracking, inventory management, and payroll system
  - Includes Mermaid diagram and detailed schema documentation
  - 60+ example queries for business analytics
  - Normalized to 3NF

- **[Online Fly Shop ERD](fly_shop_erd.md)** - Entity Relationship Diagram for an e-commerce fly fishing shop
  - 25 tables covering products, customers, orders, inventory, and fly-specific data
  - Specialized tracking for fly patterns, target species, and water conditions
  - Complete e-commerce flow: cart → order → payment → shipping
  - Product variants (size, color, weight ratings) and multi-image support
  - 50+ interesting questions including sales analytics and fly recommendations
  - Normalized to 3NF

## Viewing Diagrams

### Mermaid Diagrams
This repository uses [Mermaid](https://mermaid.js.org/) for creating diagrams. You can view them in:

- **GitHub**: Mermaid diagrams render automatically when viewing `.md` files
- **VS Code**: Install the [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid) extension
- **Online**: Use the [Mermaid Live Editor](https://mermaid.live/)

## Structure

Each diagram is contained in its own markdown file with:
- Overview and description
- Visual diagram (Mermaid syntax)
- Detailed documentation
- Example queries or use cases (where applicable)

## Technologies

- Markdown for documentation
- Mermaid for diagram generation
- Git for version control

## License

This project is for educational and reference purposes.
