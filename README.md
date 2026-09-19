# Architecture-Directed AI Engineering

*Architects, designers, and Product shape the plan. Engineers establish how it can work. AI agents carry out the construction.*

Imagine handing a robotic construction crew a hospital floor plan and saying, “Build this.”

They have excellent tools. They work incredibly fast. They can put up walls, run wiring, and install plumbing with remarkable efficiency.

They follow the plan precisely. By the time the customer walks through the finished space, the walls, wiring, plumbing, and finishes are already in place.

Then someone realizes that a wall blocks a route the staff need to use every day. It is exactly where the plan said to put it. Nobody recognized the problem before construction was complete.

The crew built what was asked. Now part of that work must be torn out and built again.

The faster the crew builds, the sooner an unanswered question becomes a wall in the wrong place. Other work then depends on that wall. A mistaken assumption becomes something expensive to undo.

AI can create the same effect in software while faithfully following our instructions. A team specifies a workflow, agents implement it, and the checks confirm that it behaves as requested. Only when stakeholders see the completed experience do they realize that the workflow does not fit how customers actually work. The team must revise the design, dismantle affected implementation, rebuild, and validate again.

Slower implementation can leave time for questions, conversations, and discoveries while work is still taking shape. When agents compress construction, that opportunity can shrink. A feature may be finished before the next conversation that would have changed its design. We can no longer rely on implementation time to provide enough room to think through what we should build.

**The faster AI can build, the more important it becomes to validate what we are asking it to build before construction begins.**

That means moving more discovery into planning: walking through user journeys, challenging assumptions, examining dependencies, and testing uncertain ideas with focused prototypes. The next increment needs a plan that people have evaluated together before agents turn it into a completed implementation.

Without that preparation, the cycle of building, discovering the wrong outcome, tearing down, and rebuilding can make AI-driven delivery more expensive than traditional human development. Better planning up front protects the speed we gain from AI by reducing how often we have to build the same thing twice.

**What if building software with agentic AI worked more like constructing a building?**

![Alt text](images/arch2bot.png)

The customer begins with a purpose. An architect helps translate that purpose into a design. Designers shape how people will experience the space. Engineers establish whether the design can support its intended loads, connect to essential systems, and operate reliably. The team considers the site, available utilities, and applicable building and zoning requirements.

A general contractor coordinates construction. Specialist crews carry out the work. Inspections establish whether the result meets the agreed requirements.

Now imagine that construction crew is made of AI agents.

Product represents customer needs, business outcomes, and priorities. Architects define system responsibilities and relationships. Designers shape workflows and experiences. Engineers determine how the system can meet its security, capacity, resilience, data, and operational requirements. Together, they direct the work and remain accountable for the result.

In this model, software engineering moves increasingly toward the architecture, design, planning, and technical assurance seats. Engineers apply their implementation knowledge to the plans, constraints, tradeoffs, and evidence that guide construction. AI agents perform more of the coding and assembly, while also helping people explore and evaluate designs.

This is **Architecture-Directed AI Engineering**: people define the intent, architecture, and engineering constraints; AI agents carry out the software construction under that direction. The shared blueprint connects human decisions to AI implementation and the evidence used to evaluate it.

The director may be one person on a small project or a coordinated team on a large platform. Either way, that direction needs a durable form that everyone can use.

It needs an architecture and blueprint package.

Part of the inspiration for the SBDK comes from where architectural knowledge has historically lived: standards in a knowledge base, designs in a diagramming tool, decisions on another team's documentation site, and implementation details in repositories. People learn where to look and whom to ask. An AI agent working in a codebase may have no access to those sources—or no idea that they exist.

Imagine handing a contractor the floor plan while leaving the building codes, structural revisions, and site survey in separate offices without telling anyone where to find them. The information exists, but it never reaches the crew doing the work.

**A standard cannot guide an agent that never receives it.** Even access alone leaves questions: Which document is authoritative? Is this the approved revision? Does this rule apply to the service being changed? What happens when two sources disagree?

The proposed **Software Blueprint Development Kit, or SBDK**, would assemble that package: product intent, architectural models, design specifications, engineering standards, applicable rules and regulatory requirements, interface contracts, decisions, and acceptance criteria, all connected to known versions.

The SBDK would connect approved sources and deliver the relevant content in a form people and agents can use together. Existing knowledge bases and diagramming tools could remain sources, with authorized integrations or reviewed, versioned exports bringing their content into the package. Each requirement would retain its source, owner, revision, and scope. Unavailable material or conflicting guidance would become visible gaps to resolve.

The result would be one coherent starting point for the work. People could evaluate the proposed outcome and design before construction, and agents would receive the applicable guidance as part of their task. Verification would then establish whether the implementation followed it, while stakeholder evaluation would test whether the result served its intended purpose.

The package tells the builders what outcome matters, which constraints apply, how the pieces fit, what they may decide, and which questions require an owner’s judgment. It also defines how the work will be checked.

Some of that material belongs to the whole organization. A shared foundation repository holds engineering standards and platform architecture. Each service references applicable versions and adds its own blueprint, behavior, contracts, and local decisions. Services reference the interfaces published by their dependencies.

The surrounding platform is the building site. Shared identity, networking, and event infrastructure are the utilities. Security, privacy, and engineering obligations supply the applicable constraints. Each service has its own purpose and design within that environment.

The SBDK would bring the relevant sources together, expose conflicts and missing decisions, and prepare a focused construction package for each change. Teams could trace an instruction back to its source and assess shared standards updates deliberately.

An orchestrating agent could then act as the general contractor, sequencing tasks and coordinating specialist agents. One might build an API, another the interface, and another the deployment configuration. Their work would share an agreed design and explicit contracts.

**The blueprint must belong to people and AI alike.**

Product needs understandable outcomes and scenarios. Architects and designers need views of responsibilities, relationships, and experiences. Engineers need precise constraints and interfaces. Agents need explicit instructions, source references, and acceptance conditions they can act on.

A useful blueprint package therefore combines clear prose and diagrams with structured models, schemas, and executable checks. Different views express the same underlying decisions. A changed interface should be reflected in the human view and the agent’s construction instructions.

People must be able to inspect and challenge what an agent is being told. Agents must be able to use those decisions without guessing which document is current or whether an important rule is hidden in a diagram. Keeping those views connected is part of the SBDK’s purpose.

**And the blueprint keeps changing as we learn.**

During construction, a customer might change the purpose of a room. A site discovery might require a foundation revision. Imagine finding granite where the team had planned to excavate. The team evaluates the implications, revises the affected design, records the reason, and coordinates the next work.

An SBDK can support the same pattern in Agile software delivery. Each increment starts from a known baseline and an agreed change. The team explores the proposed outcome, validates the design, and updates the relevant behavior, contracts, and constraints before agents implement the increment. Feedback from the result informs the next revision.

Planning focuses on the next meaningful increment, with enough architectural context to understand its wider effects. Walkthroughs, mockups, and focused prototypes give the team deliberate opportunities to learn before committing to full implementation. New discoveries can still require revisions during construction; the blueprint keeps those changes coordinated. Agile learning continues, with more of it deliberately brought forward into design as construction accelerates.

The exciting possibility is that every revision can preserve its reasons as well as its results.

Consider a building designed with a load-bearing wall. Years later, the owner wants an open floor plan. Engineers redesign the support arrangement, and a beam takes over a role previously served by the wall.

Another decade passes. A new owner wants to remodel again. The beam is in the way.

“Why is this here?”

The people who made the decision have moved on. The current drawing shows the beam, but the reason for it has disappeared.

Now imagine a living blueprint that links the original wall, the renovation request, the engineering decision, the revised support design, and the inspection record. An AI agent could quickly retrieve that history and explain: “This beam was introduced when the wall was removed. It carries a load that the original wall supported. Changing it requires a revised support design.”

The agent could identify affected elements and help engineers explore alternatives. Engineers would still validate the current conditions and any proposed structural change.

Software is full of equivalent beams: an awkward data boundary, an extra processing step, a compatibility layer, a queue that seems unnecessary. Each may exist because of a constraint that is no longer obvious.

Suppose a queue was introduced after a downstream service could not handle peak traffic. Years later, an agent asked to simplify the architecture could retrieve that decision, identify the buffering and recovery requirements, and propose evidence needed to evaluate a replacement. It could also ask whether the original capacity constraint still exists.

**That is the power of preserving architectural memory: future work can begin with the reasons behind the system.**

AI also makes maintaining that memory more practical. Under delivery pressure, people can defer documentation until the details are difficult to reconstruct. The discussion, the rejected alternative, and the reason for a compromise may never make it into the permanent record.

An agent can draft that record while the relevant context is available. As part of each change, it can capture the problem, the alternatives actually considered, the chosen approach, its stated rationale, and the consequences. It can link the decision to affected blueprint elements, code changes, and test results, then propose updates when later work supersedes it. Automating this repetitive work can make documentation faster and more consistent than relying on people to write it all manually.

In the construction analogy, the crew would arrive with a project recorder: when the wall becomes a beam, the revised plan and the reason for the change would travel together. The owner would review the record while the decision was still fresh.

The SBDK would make that record part of completing the change. Agents prepare and maintain it; responsible people confirm consequential decisions and their rationale. When the reason is missing, the agent asks or records the uncertainty. This gives future teams a maintained history they can use to plan the next renovation.

For this to be trustworthy, the records must distinguish what was proposed, what was approved, what was built, and what was actually deployed. Decisions should link to affected components, implementation changes, and verification evidence. Missing history should remain an explicit gap, rather than becoming a plausible story invented by an agent.

Inspections complete the loop. Contract tests check interfaces. Security tests probe access boundaries. Load and recovery tests evaluate operational requirements. Human review addresses tradeoffs and qualities that automated checks cannot establish. Results stay associated with the version tested.

A plan directs construction. Evidence helps establish whether construction followed the plan. Production feedback helps determine what to change next.

We can start this practice today with versioned architecture files, shared standards, explicit contracts, decision records, and existing verification tools. The SBDK is the proposed toolkit for making their assembly, use, and traceability repeatable.

The opportunity extends across the life of the software: clearer direction before construction, coordinated implementation during it, and informed renovation years afterward.

**As AI takes on more of the building, our ability to design, direct, and understand what we build becomes more valuable.**

Let the robots build. Give people and robots a blueprint they can understand together—and a record of why it became that way.
