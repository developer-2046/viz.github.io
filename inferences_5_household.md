# Inference Sheet: household (Rank 5)
**Grouping**: Low(<25%) vs High(>75%)
**Subset**: Education level=Post-Graduate Education
**Metrics**: AUC=0.73, KNN=0.56, CentroidDist=0.09

## A) Plain English Summary
This plot shows the relationship between microbiome composition and Group A/B defined by household. There is substantial overlap between the groups, suggesting that group membership is associated with moderate differences in composition. Dispersions are similar.

## B) Supported Inferences
- There is an association between the axes and the grouping variable (AUC = 0.73).
- There is substantial overlap; group membership does not deterministically determine composition.
- Group composition is distinct but not perfectly separable.
- Within-group variability is comparable to between-group differences.
- The groups are largely mixed in this view.

## C) Not Supported Inferences
- This proves that the microbiome causes the group difference.
- This identifies specific microbes driving the difference (requires feature loading analysis).
- This indicates Group A is healthier than Group B.
- This predicts an individual's group membership with high certainty (overlap prevents this).
- Distance in this plot equals 'biological distance' in all contexts.

## D) Cannot Tell From This Plot
- Whether the apparent difference remains after controlling for confounders (e.g. age, diet).
- Whether this pattern is driven by batch or site effects.
- Whether results generalize beyond this specific sample subset.
- Whether the difference is clinically relevant.

## E) Evidence Needed for Causality
- Longitudinal data showing changes within individuals over time.
- Randomized intervention studies to test causality.
- Replication in an independent cohort.
- Statistical adjustment for potential confounders.

## F) Misconceptions
- Misconception: 'The groups overlap, so there is zero difference.' (False, averages can differ even with overlap).
- Misconception: 'The separation proves biology.' (False, could be confounding).
- Misconception: 'Axis 1 is the Health Axis.' (False, axes are mathematical constructs).

## G) Multiple Choice Questions

**Q1: Which statement is supported by the visualization?**
- A: The groups are perfectly distinct with no overlap.
- B: There is substantial overlap, but centroids likely differ.
- C: Group A is caused by microbiome dysbiosis.
- D: The plot proves no relationship exists.
> **Correct Answer**: B
> *Rationale*: The KNN purity of 0.56 indicates overlap, but AUC 0.73 suggests signal.

**Q2: What can NOT be concluded from this plot alone?**
- A: The groups have different centroids in this space.
- B: There is variability within each group.
- C: The microbiome changes cause the group difference.
- D: The groups are not identical distributions.
> **Correct Answer**: C
> *Rationale*: Ordination plots show association/structure, but cannot prove causality without intervention or temporal data.

**Q3: What additional evidence would best support a causal claim?**
- A: A larger sample size in the same cross-sectional study.
- B: A 3D plot with 4 axes instead of 3.
- C: A randomized controlled trial or longitudinal intervention.
- D: Coloring the points with different colors.
> **Correct Answer**: C
> *Rationale*: Only experimental manipulation or strong longitudinal controls can establish causality.
