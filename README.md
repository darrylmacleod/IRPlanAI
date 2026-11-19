# Your IR Plan Has A Gap. It's Called AI.

Slides and a fill-in AI incident response plan template from my talk at BSides Ottawa 2026 (November 19–20, 2026).

Speaker: Darryl MacLeod, vCISO at Kobalt.io | darryl.macleod@kobalt.io

About the talk

Your incident response plan assumes something breaks and an alarm fires. AI doesn't fail that way, and attackers who use AI don't wait for your triage meeting. Models drift, agents get hijacked, data leaks through tools nobody approved, and AI-run intrusions finish in hours.

The talk covers:

Five failure modes specific to AI: silent failure, model drift, attacks on the AI itself (prompt injection, data poisoning, tool hijack), harm in the outputs, and shadow AI leakage.

Attacks from outside: AI used as the attacker's weapon, your AI stack (GPU clusters, agent builders, model keys) as the target, why most IR plans miss both, and why that's about to change.

Two incidents that are easy to miss: an agent hijacked through a support ticket, and biased automated decisions.

What the plan has to add: severity tiers, roles, a six-phase lifecycle, evidence, and controlled recovery.

The bottom line: you don't replace your IR plan, you extend it. It has to run at machine speed and cover your AI systems.

What's in this repo
File	What it is
IR_Plan_AI_Gap.pdf- The slide deck as presented (25-minute slot, 26 slides).
AI Incident Response Plan Template.docx	- The AI incident response plan template that goes with the talk. Fill it in and adapt it to your organization.

Using the template

The template extends your existing incident response plan. It doesn't replace it. Each section matches a part of the talk:

Section	Covers
1. Document control and scope	Owner, version, what counts as an in-scope AI system
2. AI system inventory	Owner, data, tools, kill switch, fallback and logging for every AI system, including GPU clusters, agent builders and model keys
3. What counts as an AI incident	Triggers for the five failure modes and the two kinds of outside attack
4. Severity tiers	P1–P4 internal targets (P1: respond in 15 min, contain in 1 h, report internally in 4 h)
5. Roles and decision authority	Including the roles most plans leave out: AI System Owner, DPO, Compliance, Risk Committee
6. Six-phase lifecycle	A checklist for each phase, from detection to post-incident review
7. Notification obligations	Canadian and international reporting clocks, with links to the sources
8. Evidence and logging	What to log on every request and what to capture as soon as you detect a problem
9. Controlled recovery	Shadow mode, close monitoring, human oversight, and the Risk Committee sign-off gate
10. Scenario playbooks	Agent hijack, biased decisions, shadow AI leak, AI stack compromise and LLMjacking, AI-accelerated intrusion
11. Gap self-assessment	For each category: what tells us it's happening, who owns it, and how we get back

Appendices	

Incident record form, related instruments, sources

Getting started:

Replace every [bracketed] field with your own values.
Fill in the AI system inventory (section 2) first. If a system isn't listed, it has no owner and no off switch.
Use the gap self-assessment (section 11) to check your current plan against the seven categories.
Set your severity targets and pre-authorized shutdown rules ahead of time, not during an incident.
Run a tabletop exercise on at least one scenario from section 10.

Regulatory references

The notification clocks in the template were checked against primary sources on November 19, 2026. 

Regulations change. Check every clock with your legal counsel before you rely on it.

Disclaimer

This material is for education and planning only. It is not legal, regulatory or compliance advice. Facts about vulnerabilities and incidents mentioned in the talk are accurate as of November 17–19, 2026. Adapt the template to your organization's own risk, legal and regulatory obligations.
