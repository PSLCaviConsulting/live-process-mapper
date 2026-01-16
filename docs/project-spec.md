# Live Process Mapper - Project Specification

## Overview

Live Process Mapper is a state-of-the-art web application for creating, sharing, and analyzing business processes using visual flowcharts. The application enables teams to collaboratively design and document their workflows using an intuitive drag-and-drop interface.

## Technology Stack

### Frontend
- **Framework:** Next.js 14+ with App Router
- - **Language:** TypeScript
  - - **Styling:** Tailwind CSS
    - - **Canvas:** React Flow for process visualization
      - - **State Management:** Zustand
        - - **Form Handling:** React Hook Form + Zod
         
          - ### Backend
          - - **Framework:** NestJS
            - - **Language:** TypeScript
              - - **Database:** PostgreSQL with Prisma ORM
                - - **Authentication:** JWT + OAuth2
                  - - **API:** REST + WebSocket for real-time collaboration
                   
                    - ### Infrastructure
                    - - **Containerization:** Docker
                      - - **CI/CD:** GitHub Actions
                        - - **Hosting:** Vercel (Frontend) + Railway/Render (Backend)
                         
                          - ## Core Features
                         
                          - ### 1. Process Visualization
                          - - Drag-and-drop canvas for creating flowcharts
                            - - Multiple node types: Action, Question, Answer
                              - - Custom connectors and edge styling
                                - - Zoom, pan, and minimap navigation
                                 
                                  - ### 2. Team Collaboration
                                  - - Projects organized in "Areas" (team spaces)
                                    - - Real-time collaborative editing
                                      - - Role-based access control
                                        - - Comments and annotations
                                         
                                          - ### 3. Export & Integration
                                          - - PDF and SVG export
                                            - - Jira integration (planned)
                                              - - API access for third-party integrations
                                               
                                                - ### 4. AI Analysis (Planned)
                                                - - Process optimization suggestions
                                                  - - Bottleneck detection
                                                    - - Compliance checking
                                                     
                                                      - ## Project Structure
                                                     
                                                      - ```
                                                        live-process-mapper/
                                                        ├── apps/
                                                        │   ├── web/                 # Next.js frontend application
                                                        │   │   ├── app/             # App router pages
                                                        │   │   ├── components/      # React components
                                                        │   │   ├── lib/             # Utility functions
                                                        │   │   └── styles/          # Global styles
                                                        │   └── api/                 # NestJS backend application
                                                        │       ├── src/
                                                        │       │   ├── modules/     # Feature modules
                                                        │       │   ├── common/      # Shared utilities
                                                        │       │   └── config/      # Configuration
                                                        │       └── prisma/          # Database schema
                                                        ├── packages/
                                                        │   ├── types/               # Shared TypeScript types
                                                        │   ├── ui/                  # Shared UI components
                                                        │   └── config/              # Shared configuration
                                                        ├── docs/                    # Project documentation
                                                        └── docker/                  # Docker configuration
                                                        ```

                                                        ## Development Phases

                                                        ### Phase 1: Foundation (MVP)
                                                        - Basic canvas with node creation
                                                        - - User authentication
                                                          - - Project/Area management
                                                            - - Simple export (PNG/PDF)
                                                             
                                                              - ### Phase 2: Collaboration
                                                              - - Real-time multi-user editing
                                                                - - Comments and annotations
                                                                  - - Version history
                                                                   
                                                                    - ### Phase 3: Integration
                                                                    - - Jira integration
                                                                      - - API documentation
                                                                        - - Webhook support
                                                                         
                                                                          - ### Phase 4: Intelligence
                                                                          - - AI-powered analysis
                                                                            - - Process templates
                                                                              - - Analytics dashboard
                                                                               
                                                                                - ## Design System
                                                                               
                                                                                - Based on the Truvle analysis, the design follows these principles:
                                                                                - - Clean, minimal interface
                                                                                  - - Dark mode primary with light mode support
                                                                                    - - Node colors distinguish types (Action: blue, Question: amber, Answer: green)
                                                                                      - - Consistent spacing scale (4px base)
                                                                                        - - Inter font family
