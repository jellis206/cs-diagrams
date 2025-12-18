# Claude Context for CS Diagrams Project

## Project Overview
This repository contains computer science diagrams, primarily Entity Relationship Diagrams (ERDs) for database schema design. Each diagram is educational and serves as a reference for database design patterns.

## Core Preferences

### Documentation Format
- **All content MUST be in Markdown files** (.md)
- No other documentation formats should be used
- Each diagram/schema gets its own dedicated markdown file

### Diagrams and Design
- **All diagrams MUST use Mermaid syntax**
- Primary diagram type: Entity Relationship Diagrams (ERD)
- Mermaid code blocks should be clearly marked with ```mermaid
- Diagrams should render in GitHub, VS Code (with extension), and Mermaid Live Editor

## Project Structure

### File Organization
```
/
├── README.md                    # Project overview and navigation
├── [topic]_erd.md              # Individual ERD files
└── claude.md                    # This file
```

### ERD File Structure
Each ERD markdown file should contain:

1. **Title and Overview**
   - Brief description of the system/domain
   - Key features and scope

2. **Mermaid ERD Diagram**
   - Complete visual representation
   - Use Mermaid erDiagram syntax
   - Show all entities and relationships

3. **Detailed Schema Documentation**
   - Table-by-table breakdown
   - Column specifications (name, type, constraints)
   - Relationships and foreign keys
   - Indexes and constraints

4. **Example Queries**
   - 50-60+ interesting SQL queries
   - Business analytics questions
   - Complex joins and aggregations
   - Demonstrate practical use cases

5. **Normalization Notes**
   - Target: 3NF (Third Normal Form)
   - Document design decisions

## Design Standards

### Database Design
- **Normalization**: All schemas normalized to 3NF
- **Naming Conventions**:
  - Tables: lowercase with underscores (e.g., `customer_addresses`)
  - Primary keys: `id` (integer, auto-increment)
  - Foreign keys: `[table_name]_id` (e.g., `customer_id`)
  - Timestamps: `created_at`, `updated_at`
  - Soft deletes: `deleted_at`

### Entity Relationships
- One-to-Many: Most common, clearly documented
- Many-to-Many: Use junction tables
- One-to-One: Use sparingly, document reasoning

### Common Patterns
- **Audit Fields**: Most tables include `created_at`, `updated_at`
- **Soft Deletes**: Include `deleted_at` where appropriate
- **Status Fields**: Use enums or lookup tables
- **Addresses**: Separate table for flexibility
- **Money Fields**: Use DECIMAL(10,2) or appropriate precision

## Content Guidelines

### When Creating New Diagrams
1. Choose a clear, realistic domain (e.g., e-commerce, service business)
2. Identify 20-30 core tables
3. Create comprehensive Mermaid ERD
4. Document each table with full schema
5. Write 50+ example queries showcasing the design
6. Ensure 3NF compliance

### Query Examples Should Include
- Basic CRUD operations
- Complex joins (3+ tables)
- Aggregations and GROUP BY
- Window functions where appropriate
- Business intelligence queries
- Performance-conscious examples

## Technologies
- **Markdown**: Primary documentation format
- **Mermaid**: Diagram generation (ERD syntax)
- **Git**: Version control
- **SQL**: Query examples (PostgreSQL/MySQL compatible)

## Workflow Preferences

### When Asked to Create Designs or Diagrams
1. Always use Mermaid syntax
2. Always create/update markdown files
3. Never suggest external tools or formats
4. Keep everything in the repository

### When Modifying Existing Diagrams
1. Read the existing file first
2. Maintain consistent structure
3. Update both diagram and documentation
4. Ensure Mermaid syntax remains valid

## Quality Standards
- **Completeness**: Each ERD should be production-ready
- **Clarity**: Clear table and column names
- **Practicality**: Real-world applicable schemas
- **Documentation**: Every design decision explained
- **Examples**: Demonstrate all major features

## Future Additions
New diagrams can cover:
- Different business domains
- System architecture diagrams (using Mermaid flowcharts/sequence diagrams)
- Data flow diagrams
- Class diagrams for OOP design
- Any CS concept that benefits from visual representation

All additions must follow the markdown + Mermaid format.
