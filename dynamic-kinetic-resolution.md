# Sharp Purity Bounds and Optimal Racemization Control in Dynamic Kinetic Resolution

Date: 2026-11-25. AI-assisted preliminary mathematical research.

**Status:** Conditional mathematical result; independent novelty review and experimental validation outstanding. Expert feedback requested from Dr. John Andraos on 2026-11-25. This is not a peer-reviewed publication.

## Model

Initially R(0)=S(0)=1/2. Substrates interconvert symmetrically at rate r(t) and react irreversibly to distinct desired and undesired products at rates k1(t)=E k2(t) and k2(t)>0, respectively. Assume E>1 is fixed, 0 <= rho(t)=r(t)/k2(t) <= rho_max, rates are locally integrable and the target conversion is reachable. No side reactions or product interconversion.

The equations are R'=-k1 R-r R+r S and S'=-k2 S+r R-r S. Product rates are k1 R and k2 S.

## Fixed-conversion optimality theorem

Maintaining rho=rho_max throughout maximizes desired-product fraction at every reachable fixed positive conversion, among admissible schedules.

**Proof.** Let M=R+S, z=S/M and v=-ln M. Then

dz/dv = [(E-1)z(1-z)-rho(2z-1)]/[E(1-z)+z].

The interval [1/2,1] is invariant: the vector field points inward at its endpoints. On that interval it is nonincreasing in rho. Scalar ODE comparison at equal v gives z_max(v) <= z_other(v), where max denotes the constant maximal racemization ratio. The instantaneous undesired fraction per unit conversion is z/[E(1-z)+z], increasing in z. Integrating from zero to the target conversion proves the claim.

## Complete-conversion formula (constant rates)

Integrate the linear kinetic equations to extinction. The integrated R and S are (k2+2r)/(2D) and (k1+2r)/(2D), where D=k1*k2+r*(k1+k2). The signed product enantiomeric excess is therefore

ee = rho*(E-1)/(E+rho*(E+1)).

For target 0<e<1, finite rho is possible only when E>(1+e)/(1-e); the minimum ratio is

rho_min=e*E/[E-1-e*(E+1)].

Example: E=100 and rho=10 gives ee=89.19%, or 94.59% desired product in this model.

## Scope and prior art

This does not establish optimality for varying selectivity, catalyst budgets, fixed elapsed time, nonlinear kinetics, side reactions or asymmetric interconversion. Numerical examples are model predictions, not measured chemical performance. The constant-rate formula may be established prior art; the bounded time-dependent fixed-conversion comparison is the candidate contribution. Related work: John Andraos, *Quantification and Optimization of Dynamic Kinetic Resolution*, https://doi.org/10.1021/jp0272365. Originality is not established.

Next steps: independent literature and proof review, calibration against measured rate constants, and experimental validation.
