#Miscellaneous
# Windows PowerShell
Get-ChildItem -Directory -Recurse | ForEach-Object { New-Item -ItemType File -Force -Path ($_.FullName + "\.gitkeep") }

springboot-learning/
├── README.md

├── 00-roadmap/                # what you plan to learn
│   ├── backend-roadmap.md
│   ├── springboot-roadmap.md

├── 01-daily/                  # learning journal (raw progress)
│   ├── 2026-03-31.md
│   ├── 2026-04-01.md

├── 02-concepts/               # clean, structured knowledge
│   ├── core/
│   │   ├── spring-core.md
│   │   ├── beans-lifecycle.md
│   │   ├── dependency-injection.md
│   ├── web/
│   │   ├── rest-api.md
│   │   ├── request-lifecycle.md
│   ├── security/
│   │   ├── jwt.md
│   │   ├── spring-security.md
│   ├── database/
│   │   ├── jpa.md
│   │   ├── hibernate.md
│   │   ├── transactions.md
│   ├── architecture/
│   │   ├── layered-architecture.md
│   │   ├── microservices.md

├── 03-syntax/                 # quick reference (VERY IMPORTANT)
│   ├── annotations.md
│   ├── common-patterns.md
│   ├── cheatsheet.md

├── 04-errors/                 # debugging knowledge base
│   ├── spring-errors.md
│   ├── database-errors.md
│   ├── api-errors.md

├── 05-projects/               # real implementations (portfolio)
│   ├── auth-api/
│   │   ├── overview.md
│   │   ├── architecture.md
│   │   ├── api-design.md
│   │   ├── problems-faced.md
│   ├── erp-module/
│   │   ├── overview.md

├── 06-snippets/               # reusable code (goldmine)
│   ├── controller.md
│   ├── service.md
│   ├── repository.md
│   ├── jwt-filter.md

├── 07-tools/                  # tools you use
│   ├── postman.md
│   ├── docker.md
│   ├── git.md

├── 08-testing/                # testing knowledge
│   ├── junit.md
│   ├── mockito.md
│   ├── api-testing.md

├── 09-performance/            # optimization & scaling
│   ├── query-optimization.md
│   ├── caching.md

├── 10-devops/                 # deployment & infra
│   ├── docker.md
│   ├── ci-cd.md
│   ├── deployment.md

├── 11-design-patterns/
│   ├── singleton.md
│   ├── factory.md
│   ├── builder.md

├── 12-api-design/
│   ├── rest-best-practices.md
│   ├── versioning.md

├── 13-database-design/
│   ├── normalization.md
│   ├── indexing.md

├── 14-security-deep-dive/
│   ├── oauth2.md
│   ├── csrf.md
│   ├── cors.md

├── 
│   ├── questions.md
│   ├── system-design.md

└── notes.md                  # scratchpad

$folderList = @("auth-api","erp-module"); foreach ($folderList in $folderList) {New-Item -ItemType Directory -Name $folderList}

$files = @("postman.md","docker.md","git.md"); foreach ($files in $files) {New-Item -ItemType File -Name $files}