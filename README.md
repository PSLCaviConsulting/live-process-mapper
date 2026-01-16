# Live Process Mapper

A state-of-the-art live process mapping application for creating, sharing, and analyzing business processes. Built with Next.js, NestJS, React Flow, and PostgreSQL.

## Features

- **Visual Process Editor** - Drag-and-drop canvas with intuitive node-based workflow creation
- - **Multiple Node Types** - Action, Question, and Answer nodes for comprehensive process mapping
  - - **Real-time Collaboration** - Work together with your team on process designs
    - - **Team Management** - Organize projects in Areas with role-based access control
      - - **Export Options** - Export processes as PDF or SVG
        - - **AI Analysis** (Coming Soon) - Get intelligent suggestions for process optimization
         
          - ## Tech Stack
         
          - | Layer | Technology |
          - |-------|------------|
          - | Frontend | Next.js 14+, React, TypeScript, Tailwind CSS |
          - | Canvas | React Flow |
          - | Backend | NestJS, Prisma |
          - | Database | PostgreSQL |
          - | Monorepo | Turborepo |
         
          - ## Project Structure
         
          - ```
            live-process-mapper/
            ├── apps/
            │   ├── web/          # Next.js frontend
            │   └── api/          # NestJS backend
            ├── packages/
            │   ├── types/        # Shared TypeScript types
            │   ├── ui/           # Shared UI components
            │   └── config/       # Shared configuration
            ├── docs/             # Documentation
            └── docker/           # Docker configuration
            ```

            ## Getting Started

            ### Prerequisites

            - Node.js 18+
            - - npm 9+
              - - PostgreSQL 15+
               
                - ### Installation
               
                - 1. Clone the repository:
                  2. ```bash
                     git clone https://github.com/PSLCaviConsulting/live-process-mapper.git
                     cd live-process-mapper
                     ```

                     2. Install dependencies:
                     3. ```bash
                        npm install
                        ```

                        3. Set up environment variables:
                        4. ```bash
                           cp .env.example .env.local
                           ```

                           4. Start the development servers:
                           5. ```bash
                              npm run dev
                              ```

                              ## Development

                              ```bash
                              # Run all apps in development mode
                              npm run dev

                              # Build all apps
                              npm run build

                              # Run linting
                              npm run lint

                              # Run tests
                              npm run test
                              ```

                              ## Documentation

                              For detailed documentation, see the [docs folder](./docs).

                              ## License

                              This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

                              ## Contributing

                              Contributions are welcome! Please feel free to submit a Pull Request.
