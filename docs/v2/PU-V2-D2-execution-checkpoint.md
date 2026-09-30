# POROS UNIVERSE V.2 — D2 Execution Checkpoint

**Status:** BLOCKED AT DECISION GATE  
**Scope:** POROS UNIVERSE V.2 only  
**Separation:** V.2 is maintained independently from V.1.

## 1. Authority of this record

This record operationalizes the current V.2 baseline without promoting proposals into approved architecture.

The V.2 workspace is explicitly separate from V.1. Changes in V.2 do not automatically modify V.1, and V.1 material may enter V.2 only through evaluation and recording.

## 2. Current D2 state

D2 cannot be LOCKED yet.

Open conditions:
- D2-3 — Tenancy hierarchy: PENDING.
- D2-4 — Execution Identity: PENDING.
- D2 — Schema & authority contract: NOT FINAL.
- D2 — Conformance & isolation tests: NOT RUN.

## 3. D2-4 proposal retained as proposal

The baseline proposes:
- persistent Agent Identity;
- unique Execution Identity per execution run;
- short-lived credentials scoped to the execution and permitted capability.

Proposed authority chain:

Delegating Principal
→ Agent Identity
→ Execution Identity
→ Permission → Action

The baseline further requires authority attenuation, traceability per run, credential scope/expiry/revocation, credential exclusion from blueprint/prompt/trace, and tenant isolation.

**Important:** these are baseline proposals/criteria, not an approved implementation contract.

## 4. Required Governor decisions

### D2-3 — Tenancy hierarchy

Available baseline choices:
1. Organization required as root tenant → Workspace → Project; no nested Organization in v1.
2. Organization required with nested Organization.
3. Defer D2-3 and analyze alternatives.

### D2-4 — Execution Identity

Available baseline choices:
1. Persistent Agent Identity + unique Execution Identity per run + short-lived credential per run.
2. Persistent Execution Identity per agent, with separate run ID.
3. Defer D2-4 and perform threat modeling first.

No option is selected by this record.

## 5. Post-decision execution sequence

Once D2-3 and D2-4 are explicitly decided:

1. Record the Governor decision.
2. Freeze the selected D2 semantic model.
3. Produce D2 Architecture Specification.
4. Produce entity/schema contract.
5. Produce authority enforcement contract.
6. Produce tenant-isolation and conformance test matrix.
7. Execute tests.
8. Collect evidence.
9. Run D2 Architecture Acceptance Gate.
10. Only after PASS may D2 become LOCKED.
11. Only then proceed to D3 — Universal Execution Interface.

## 6. Gate rule

This checkpoint does **not** authorize:
- D2 LOCK;
- implementation based on an unapproved option;
- promotion of the proposed model to canonical architecture;
- progression to D3.

## 7. Current next action

**Governor decision required for D2-3 and D2-4.**

After those decisions are supplied, execution can continue sequentially without reopening already-set V.2 separation parameters unless new evidence creates a justified change request.
