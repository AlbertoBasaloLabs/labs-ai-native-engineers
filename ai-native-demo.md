## I - Human In The Loop

### 1 - Vibe Coding to AI-DD
- **1.1 Vibe Coding**
  - `feat(rockets): scaffold CRUD via short vibe-coding loops`
- **1.2 Prompt Engineering**
  - `feat(launches): schedule a launch for a rocket, single well-crafted prompt`
- **1.3 AI-Driven Development Primitives**
  - `chore(rules): add coding rules, a skill and a spec template`

### 2 - Context Engineering
- **2.1 The Context Window**
  - `feat(launches): list scheduled launches`
- **2.2 Context Selection**
  - `feat(users): register operator and passenger accounts`
- **2.3 Dynamic Documentation**
  - `feat(launches): show launch detail with live occupancy`

## II - Human On The Loop

### 3 - Spec-Driven Development
- **3.1 Specs as Source of Truth**
  - `feat(bookings): create booking and charge mock payment`
- **3.2 From Spec to Planned Task**
  - `feat(bookings): validate seat availability before charging`
- **3.3 Writing Code is the Easy Part**
  - `test(bookings): add booking creation test suite`

### 4 - Trust but Verify
- **4.1 E2E Behavior Validation**
  - `test(bookings): add e2e booking flow validation`
- **4.2 The Fixing Loop** 🔴
  - `fix(bookings): prevent overbooking beyond seat capacity`
- **4.3 The Review Loop**
  - `refactor(obs): add centralized error handling and structured logging`

### 5 - Legacy Refactoring
- **5.1 Exploring the Legacy**
  - `docs(payments): document the undocumented mock gateway from 3.1`
- **5.2 Change Triage**
  - `feat(launches): add cancellation reason and fee`
- **5.3 Structural Refactoring** 🔴
  - `refactor(payments): replace payment DTO with Money value object`

## III - Away From Keyboard

### 6 - Harness Engineering
- **6.1 Hooks & Control Points**
  - `ci(hooks): add pre-commit lint and test hook`
- **6.2 MCP Integration**
  - `feat(mcp): connect agent to CI pipeline via MCP server`
- **6.3 Subagents**
  - `chore(agents): configure subagents for rockets and launches`

### 7 - Agent Orchestration
- **7.1 The Session Window Problem**
  - `docs(context): split domain docs into per-module context files`
- **7.2 Sequential vs Parallel**
  - `feat(users): add passenger profile update, two agents in parallel`
- **7.3 Context Sharing**
  - `feat(payments): process refunds for canceled launches, agent swarm`

### 8 - Loop Engineering
- **8.1 From Pipelines to Loops**
  - `feat(loop): add payment retry loop with backoff`
- **8.2 Stop Conditions**
  - `feat(loop): add max-retry stop condition to payment loop`
- **8.3 Away From Keyboard**
  - `feat(launches): auto-confirm launches at occupancy threshold, unsupervised`