# A Universal Rearrangement Principle for Optimal Chemical Production with Nonlinear Catalyst Deactivation

Date: 2026-11-25. AI-assisted preliminary mathematical research.

**Status:** Conditional mathematical theorem; novelty and experimental applicability not independently established. Expert feedback requested from Professor Hannsjörg Freund on 2026-11-25. Not a peer-reviewed publication.

## Model and assumptions

For reactant concentration C>0 and n independent nonnegative catalyst activities a_i, consider

C' = -C sum_i k_i(u)a_i,
a_i' = -d_i(u)f_i(a_i).

There is a finite set of operating modes u, with prescribed total exposure times T_u. The order and subdivision of the modes are free. Assume k_i(u)>=0, d_i(u)>0, f_i>=0, and well-posed dynamics that preserve nonnegative activity. Initial activities are fixed. Assume all catalyst populations admit a common weak descending ordering of R_i(u)=k_i(u)/d_i(u).

## Global optimality theorem

A schedule applying the modes in that common descending order maximizes final conversion, even among measurable schedules with arbitrarily many switches.

**Proof.** Define s_i(t)=integral_0^t d_i(u(q))dq. Since d_i>0, this is a strictly increasing clock. Then a_i satisfies da_i/ds_i=-f_i(a_i), and hence is a fixed nonincreasing function A_i(s_i) independent of the ordering. The terminal log conversion is

-log(C(T)/C(0)) = sum_i integral_0^{s_i(T)} R_i(u(t(s))) A_i(s) ds.

In clock i, each mode occupies the prescribed measure d_i(u) T_u. Thus the distribution of R_i is fixed. The Hardy-Littlewood rearrangement inequality maximizes each term by placing larger R_i earlier, since A_i is nonincreasing. By the common ordering hypothesis a single physical schedule realizes each individual maximizer. Summing proves global optimality. Since conversion is an increasing function of terminal log conversion, it too is maximized.

## Conflicting rankings

If two catalyst populations strictly disagree on the ranking of two modes and each has strictly decreasing activity, then no ordering is universally optimal across arbitrary relative population weights: the two extreme choices of weights favor opposite orders. This observation does not solve the general conflicting-ranking scheduling problem.

## Scope and prior art

The theorem does not cover coupled or concentration-dependent degradation, variable mode exposure budgets, competing products, regeneration, switching costs, or mass/heat-transfer limitations. The classical rearrangement inequality is established mathematics; originality of this particular application requires independent literature review. Related research: Xie and Freund, *Optimal reactor design and operation taking catalyst deactivation into account*, https://doi.org/10.1016/j.ces.2017.10.010.

## Next steps

Independent proof and novelty review; identify suitable experimental systems; calibrate against measured kinetics; investigate conflicting rankings. No industrial productivity improvement is asserted without experimental evidence.
