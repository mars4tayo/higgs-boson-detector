# higgs-boson-detector
https://github.com/user-attachments/assets/f8ca01f2-dce7-4224-9d40-89b34811bdf6

My Higgs Boson Detection with Machine Learning(Kaggle Competition):
The Higgs boson, theorized in 1964 and discovered in 2012 at the Large Hadron Collider (LHC), explains mass via the Higgs field. Its detection is challenging due to its rarity—about 300 Higgs events per 10^11 collisions and background noise from top quark pairs (tt̄, t is a top quark, t̄ its antiparticle) or W+jets (W boson plus jets). Machine learning (ML) enhances detection by analyzing datasets to separate signal from noise, as in the Kaggle Higgs Boson Detection 2025 challenge using ATLAS simulations.
Dataset and Important Data Features:
Higgs detection uses collision data from LHC experiments like ATLAS and CMS. Simulated datasets are vital due to scarce signal events. The HIGGS dataset (UCI Machine Learning Repository) provides 11 million Monte Carlo events, each with 28 features and a binary label (1 for signal, 0 for background), split into:
1. Low-Level Features (21):Detector measurements:
Lepton kinematics: Transverse momentum (pT, momentum perpendicular to beam), pseudorapidity (η = -ln[tan(θ/2)], θ is polar angle), azimuthal angle (ϕ, angle in transverse plane) for leptons (e.g.,from H → WW* → ℓνℓν, ℓ is lepton, ν is neutrino, WW* indicates one off-shell W boson).
Missing transverse energy: Magnitude and ϕ, showing undetected particles like neutrinos, termed MET (Missing Transverse Energy).
Jet properties: pT, η, ϕ, b-tagging (probability jet is from b-quark) for up to four jets, key for H→bb (b-quark pair).
2. High-Level Features (7): Derived quantities:
Invariant masses: m_jj (two jets), m_bb (b-tagged jets), peaking at 125 GeV/c² for Higgs signals.
Combinations: m_wwbb (mass with W bosons, b-jets), aiding resonance identification.
These features encode Higgs decay physics(leptons, jets, MET) enabling ML to distinguish signals from backgrounds.

Physics Insights and ML Integration:
ML boosts Higgs detection by finding complex patterns.
Techniques include:
Neural Networks: Multi-layer perceptrons (MLPs), graph neural networks (GNNs) capture non-linear correlations.
Ensemble Methods: XGBoost, random forests manage class imbalance, reaching 74% accuracy.
Unsupervised Learning: Autoencoders detect anomalies, aiding di-Higgs searches.
ML reveals kinematic differences, like m_bb peaks, missed by traditional cuts. Debate persists with regards to physics-based features (e.g.,masses) which offer interpretability, while data-driven methods boost performance. ML excels at background rejection, potentially uncovering new physics in di-Higgs studies.
Finally
As LHC datasets grow, ML’s role in Higgs detection will expand, focusing on interpretable models, bias mitigation, and generative methods to advance particle physics.
Notations:
tt̄: Top quark (t), anti-top quark (t̄) pair.
W+jets: W boson with jets.
H→WW→ℓνℓν: Higgs to two W bosons (one off-shell, WW), then leptons (ℓ), neutrinos(ν).
H→bb: Higgs to bottom quark (b), anti-bottom quark (b̄) pair.
MET:Missing Transverse Energy
