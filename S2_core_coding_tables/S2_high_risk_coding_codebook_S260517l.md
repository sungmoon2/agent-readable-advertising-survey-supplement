# S2 High-Risk Coding Codebook Clarification

Created: 2026-05-17

## Purpose and Boundary

This file clarifies how to read high-risk interpretive fields in the S2 core coding table for the 87-paper core corpus. It documents field definitions and boundary rules used for traceability in the survey synthesis.

This file does not report independent double coding, inter-rater reliability, Cohen's kappa, Jaccard agreement, a calibration round, or adjudication statistics. The row-level responsibility fields in S2 document distributed literature identification/coding responsibility by cluster or subset.

## Unit of Analysis

The unit of analysis is the paper-level record in the 87-paper core corpus. When a paper reports several systems, datasets, or experiments, the coding summarizes the contribution most relevant to the survey's cluster assignment and research-gap mapping.

## Primary Cluster Rule

Each core paper is assigned to one primary research cluster, C1-C6, according to the paper's main contribution in the survey:

- C1: multimodal ad understanding, ad semantics, ad classification, ad QA, captioning, or representation of ad meaning.
- C2: ad creative generation, creative-quality evaluation, CTR/engagement-oriented generation, or creative production workflows.
- C3: policy-relevant ad interpretation, disclosure detection, claim verification, deceptive-claim analysis, or moderation.
- C4: LLM-native advertising, conversational advertising, ad insertion into generated responses, ad auctions in LLM settings, or detection of generated/native ads.
- C5: shopping, commerce, or web-agent benchmarks and agent behavior in commerce or ad-adjacent shopping settings.
- C6: agent safety, prompt injection, pop-up or ad-mediated attack surfaces, web-agent hijacking, safety benchmarks, or defenses against agent compromise.

If a paper spans multiple clusters, the primary cluster follows the contribution whose research landscape would be incomplete without the paper. Borderline records are interpreted with respect to the survey's central question: how human-facing advertisements become machine-consumed inputs for AI commerce agents.

## Secondary Cluster Rule

Secondary cluster links are interpretive cross-references. A paper is secondary-linked only when it substantively contributes to another cluster's synthesis, not when it merely mentions adjacent topics. Secondary links are used for synthesis and gap interpretation; they are not counted as additional primary cluster papers.

## Evidence-Level Rule

Evidence levels distinguish source type:

- E1: peer-reviewed paper or formally accepted proceedings publication.
- E2: preprint or not-yet-peer-reviewed manuscript.
- E3: standards, specifications, protocol documentation, or official technical documentation.
- E4: industry report, product documentation, blog, announcement, or other non-peer-reviewed industry source.

C1-C6 counts refer to E1/E2 research papers. C7/C8 are infrastructure corpora based on E3/E4 sources and are not research-paper clusters.

## Output-Form Rule

Output form records what the reviewed paper's system or benchmark produces or evaluates. Common output forms include:

- labels, categories, or tags;
- captions or text descriptions;
- QA answers or explanations;
- moderation decisions or violation labels;
- temporal localization or reasoning traces;
- CTR, engagement, quality, or benchmark-success metrics;
- agent actions or task-completion outcomes;
- attack success / safety outcomes.

For this survey, an output is not treated as a full agent-readable ad representation unless it provides a structured, machine-parseable record that connects ad creative evidence, product/offer facts, claims, disclosure/sponsor/provenance, policy or risk signals, temporal validity, uncertainty, and action constraints.

## Agent-Tested Rule

A paper is coded as agent-tested when it evaluates an autonomous or semi-autonomous agent that perceives, navigates, reasons, invokes tools, or performs web/commerce actions. LLM-only or VLM-only evaluation is not treated as agent-tested unless the model is embedded in an agentic workflow with actions or tool/environment interaction.

## Standard-Compatibility Rule

Standard compatibility records whether a paper or source directly uses, evaluates, maps to, or is constrained by an ad-tech standard or agentic commerce protocol. General mention of standards does not imply compatibility. C7/C8 sources may provide delivery, provenance, consent, communication, payment, or commerce-flow infrastructure without providing AARS-equivalent creative, claim, evidence, or action-constraint fields.

## Threat-Model and Defense-Tested Rule

Threat-model coding records the attacker capability, target surface, and objective when applicable. Defense-tested coding distinguishes:

- no defense evaluated;
- prompt-only or instruction-level defense;
- generic prompt-injection or tool-filtering defense;
- detector or benchmark evaluation;
- ad-specific or ad-surface-specific defense.

A paper is treated as addressing the G7 agent-side ad-defense gap only if it proposes, evaluates, or directly motivates a defense mechanism for advertising, sponsored content, pop-ups, disclosure verification, ad-derived action constraints, or comparable ad-like commercial surfaces. Generic prompt-injection defenses are not counted as purpose-built agent-side ad-filtering defenses unless they explicitly handle advertising or ad-like commercial surfaces.

## RQ and G1-G10 Link Rule

RQ and gap links are interpretive synthesis fields. A paper is linked to an RQ or G1-G10 gap only when its findings, limitations, benchmark design, or system boundary provide direct evidence for that question or gap.

The highest-risk gap links are:

- G1/G10: absence of evidence-grounded, temporally valid, actionable agent-readable ad representations.
- G2/G3/G5: absence of causal and consequential evaluation from ad exposure to belief, action, and commercial outcome.
- G7: absence of purpose-built general agent-side ad-filtering defenses in the reviewed C6 corpus.
- G8/G9: governance, accountability, and incentive gaps across ad exposure, agent authority, provenance, and commercial action.

## Corpus-Bounded Negative Claims

Negative claims are interpreted as corpus-bounded claims. They mean that the reviewed corpus and the associated coding records did not identify a system, benchmark, or standard satisfying the specified condition. They are not claims that no such work exists anywhere outside the reviewed corpus.

## Relationship to S2 Responsibility Records

The S2 row-level responsibility fields record distributed literature identification/coding responsibility and completion status. They support traceability of who checked which cluster/subset, but they are not an inter-rater reliability dataset.
