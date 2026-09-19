# Frank Santermans
**Audio Engineer & AI System Architect**

Bridge between 20+ years of broadcast/studio audio engineering and modern AWS-native AI processing pipelines. Specializing in autonomous audio processing, dynamic AI host systems, and custom DSP integration.

### What I Do
* **Architecting Audio Pipelines:** Designing scalable, event-driven workflows that merge classical DSP with generative AI tools (voice synthesis, isolation, restoration).
* **AI & Host Logic:** Developing contextual host systems that interpret media parameters, evaluate user profiles, and generate dynamic processing plans.
* **Production Systems:** Building AWS-native (Lambda + S3) infrastructure engineered for reliable, production-grade audio delivery.

---

## Featured Project: Audia Lab (System Architecture)

**Audia Lab** is an event-driven, AWS-native audio post-production engine. It decouples customer interaction, job orchestration, and execution into a highly scalable three-layer architecture.

### Architectural Overview (Factory Floor)

<img width="998" height="683" alt="audIA-lab system architecture" src="https://github.com/user-attachments/assets/39d29abc-146e-48f1-8b72-2b8834cee579" />


---

### Core Architecture Highlights

* **Client Layer**: Ingests multi-modal media (audio, video, text, image). An **AI Host** loads the client's historical profile (`Customer Card`) alongside acoustic findings from **Intake Analysis** to write a contextual processing plan (`plan.json`).
* **Control Plane**: Decouples job contract execution. The **Jobs Engine** pairs the plan with assets from the **Library**, which the **Orchestrator** sequences and manages under execution limits.
* **Processing Floor**: Serverless runtime on **AWS Lambda + S3** (`eu-north-1`). Operates an integrated floor combining native DSP (repair, mix, spatial audio) with generative AI tools (ElevenLabs voice synthesis/dubbing, Lalal.ai stem isolation, music/SFX generation).

---

*Note: The underlying repository (`audialab-backbone`) contains proprietary production code and is kept private. Technical architecture discussions available upon request.*
