<!-- ⊕ 𝔹 ∈ -->

<style>
font-size: 15pt
</style>

Semigroups
==========

It's a pair *(⊕,𝔹)*, where 𝔹 is a set and ⊕ is a binary function ⊕ : 𝔹 → 𝔹 → 𝔹 (or ⊕:𝔹×𝔹↦𝔹 in highschool algebra notation).

such that

∀ a,b,c ∈ 𝔹 ⟹ (a ⊕ b) ⊕ c = a ⊕ (b ⊕ c)

eg:
  - 1 + 2 + 3
  - 1 \`max\` 2 \`max\` 3
  - 1 > 2 > 3
  - 1 \`min\` 2 \`min\` 3
  - 1 > 2 > 3
  
Not semigroups:
  - 1 - (1 - 1) ≠ (1 - 1) - 1
  
  
Semigroupoid:
  -  1 `const` (2 `const` 3) = (1 `const` 2) `const` 3 
