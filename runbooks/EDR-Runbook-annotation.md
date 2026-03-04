EDR Runbook Annotation

What is this document?

This is an Endpoint Detection and Response (EDR) deployment and operations runbook produced during my role as a full time admin. It covers the full lifecycle of EDR agent management across Windows, macOS, and Linux environments including package deployment, VSS configuration, log collection, performance troubleshooting, and day-to-day IT operations procedures.

The document has been sanitized for portfolio use. The EDR vendor name has been replaced throughout with `[EDR VENDOR]`, management console UI screenshots have been replaced with descriptive placeholders, and all organizational branding has been removed. All procedural and technical content is unmodified.

What problem does this document solve?

EDR operations and maintenance activities are frequently underdocumented in environments where the technology was adopted reactively. Engineers know how to install the agent but no one will have written down what to do when certain common issues arise, such as CPU spikes after deployment, how to handle VSS conflicts on Windows Server, or what the correct log collection procedure is for a Linux endpoint that isn't checking in. This runbook was written to give local and regional IT and security operations leaders and staff a single reference that covers not just initial deployment but the day-to-day operational requirements of maintaining EDR at scale.

What decisions did I make and why?

The runbook is structured to follow the natural sequence of an EDR deployment engagement rather than organizing by platform or feature. Deployment comes before troubleshooting; troubleshooting comes before day-to-day operations. This mirrors how the intended audience would actually encounter the tool, and reduces the toil of those users finding the right answer under pressure or when business operations are disrupted due to an EDR issue.

The compatibility tables covering Windows versions, macOS versions, and Linux distributions with ARM architecture notes were included explicitly because platform support gaps and feature parity discrepancies were common sources of deployment failures and, later, operational interruptions. Making this information visible at the front of the runbook surfaces it before the user drills down in troubleshooting and makes it easier to refer back to during active investigation.

The CPU debugging and ProcMon sections were written to be standalone procedures; complete enough to follow without needing to reference external documentation. This was purposefully done due to performance complaints after previous EDR deployments in production (which are the most common reason IT teams seek exceptions to deployment mandates). The goal was to have a clear, self-contained diagnostic path to reduce the likelihood of individual endpoints/agents being fully disabled out of frustration/convenience rather than properly tuned.

What was my role and scope?

I am the primary author of all procedural content, compatibility documentation, troubleshooting procedures, and operational guidance. The document was developed for internal use and subsequently maintained as a reference for local IT, offshore MSP support, regional CIOs and operations leaders, and security operations staff supporting the EDR deployment globally.

What does this demonstrate?

This document demonstrates my ability to translate security tooling into operational documentation that non-security IT staff can follow without vendor support. Runbook writing for security tools requires bridging two audiences: security engineers who understand why the controls exist and IT operations staff who need to implement and maintain them with other time, resource and business-needs restraints. 
