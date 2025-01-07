# Lab: Predicting and Interpreting IR Spectra

---

## Introduction

Infrared (IR) spectroscopy is a powerful analytical technique used to identify functional groups within organic molecules based on **molecular vibrations**. When molecules absorb infrared radiation, specific bonds within the molecule vibrate at characteristic frequencies, leading to absorption peaks in the IR spectrum. By analyzing these peaks, chemists can deduce the presence of particular functional groups, aiding in the structural determination of organic compounds.

In this lab, you will use the [QOOL quantum chemistry lab](https://qool.stanford.edu) to model three organic molecules—**ethanol**, **acetone**, and **styrene**—and predict their IR spectra. You will then interpret the spectra to identify key functional groups based on the observed absorption peaks. This hands-on experience will enhance your understanding of how molecular structure influences IR spectra and how to correlate specific bond vibrations with functional groups.  

!!! tip "What is QOOL?"
    A brief overview of QOOL can be found here:  
    [https://www.youtube.com/watch?v=8Bxp9r8a1Wc](https://www.youtube.com/watch?v=8Bxp9r8a1Wc)

---

??? note "Topics Covered (McMurry 10e Ch. 12)"
    - **Structure Determination**  
    - **Reading Infrared (IR) Spectra**  
    - **Correlating Bond Vibrations to Functional Groups**  
    [Link to Chapter](https://openstax.org/books/organic-chemistry/pages/12-why-this-chapter)

---

## Objectives

**Primary Objective:**  
Utilize QOOL to predict and interpret the IR spectra of ethanol, acetone, and styrene.

**Secondary Objectives:**
- Identify and assign key absorption peaks to corresponding bond vibrations.  
- Understand the relationship between molecular vibrations and the observed IR spectra.  
- Correlate functional groups with specific IR absorption frequencies.

---

## Materials and Equipment

- Access to the **QOOL online quantum chemistry lab**  
- **Computer** with internet access  
- **Notebook** or lab report template for recording observations  

!!! info "Safety Precautions"
    Since this is a **virtual lab** using computational tools, there are no physical safety hazards.

---

## Procedure

### 1. Naming Your Molecule

!!! note "Name Your Molecule"
    Incorporate your first and last name with the molecule you build. For example, if your name is **Jamie Smith** and you choose methanol, your molecule would be named:  
    **"JamieSmith Methanol (CH₃OH)"**

=== "Examples"
    - If your name is **Alex Johnson** and you choose ethanol, name it **"AlexJohnson Ethanol (C₂H₅OH)"**.

---

### 2. Building the Molecule in QOOL

1. **Access QOOL**  
   - Log in to the [QOOL platform](https://qool.stanford.edu) using your credentials.  
   - Familiarize yourself with the molecular builder and visualization tools.

2. **Construct Your Molecule**  
   - Use the molecular builder to assemble your chosen molecule, ensuring correct connectivity and geometry.  
   - **Example (Ethanol)**:  
     - Connect two carbon atoms with a single bond.  
     - Add five hydrogen atoms accordingly.  
     - Attach a hydroxyl group (-OH) to the terminal carbon.

3. **Optimize the Geometry**  
   - Before running any calculations, **optimize** the molecular geometry to minimize energy and achieve a realistic conformation using QOOL's optimization tool.

<figure markdown="span">
  ![Example Image: Methanol Model CH3OH](https://dummyimage.com/600x400/){ width="300" }
  <figcaption>Example Image: Methanol Model CH3OH Build w/ QOOL</figcaption>
</figure>

---

### 3. Setting Up the IR Spectrum Calculation

1. **Calculation Type**  
   - Navigate to the **"Calculation"** dropdown menu.  
   - Select **"Vibrational Frequencies"** or **"Optimize + Vib Freq"** to perform vibrational frequency analysis.

2. **Choose Computational Method and Basis Set**

??? abstract "Recommended Methods for IR Spectra"
    - **B3LYP**: A popular hybrid density functional theory (DFT) method that balances accuracy and computational cost.  
    - **ωB97X-D**: A DFT method with dispersion corrections, ideal for systems where dispersion forces are significant.  
    - **PBE0**: Another reliable DFT method suitable for vibrational analysis.

??? example "For Higher Accuracy (More Computationally Demanding)"
    - **MP2**: A post-Hartree-Fock method offering greater accuracy at increased computational cost.  
    - **CCSD(T)**: A highly accurate coupled-cluster method, recommended if computational resources are not a limitation.

??? info "Recommended Basis Sets for Routine Calculations"
    - **6-31G(d)**: Includes polarization functions, providing good accuracy while being computationally efficient.  
    - **6-311+G(d,p)**: Incorporates diffuse functions for systems with lone pairs or delocalized electrons, offering enhanced accuracy.

??? tip "For High Accuracy"
    - **cc-pVDZ, cc-pVTZ, aug-cc-pVDZ**: Correlation-consistent basis sets for precise results, though more computationally intensive.

=== "Auxiliary Basis Set"
- **None**: Appropriate for most routine calculations unless using advanced methods (e.g., explicitly correlated calculations like MP2-F12).  
  Leave this as **"None"** for standard IR spectra calculations.

3. **Charge**  
   - **For neutral molecules** (e.g., ethanol, acetone, styrene), set the charge to **0**.  
   - If working with an ion (e.g., a cation or anion), input the appropriate charge value.

4. **Multiplicity**  
   - **Singlet** (default for most organic molecules).  
   - **Doublet** (1 unpaired electron) or higher if the molecule has radicals/unpaired electrons.

5. **Unrestricted**  
   - **Leave Unchecked** for singlet spin states (default).  
   - **Check if necessary** only for radicals or open-shell systems requiring an unrestricted spin calculation.

<figure markdown="span">
  ![Example: Setting Up the IR Spectrum Calculation](https://dummyimage.com/600x400/){ width="300" }
  <figcaption>Example: Setting Up the IR Spectrum Calculation</figcaption>
</figure>

---

### 4. Running the Calculation

1. **Submit the Job**  
   - Review all settings to ensure accuracy.  
   - Submit the calculation and wait for it to complete. Note that higher-level methods and larger basis sets may require more time.

2. **Think While Waiting for QOOL (Optional)**  
   While your computational job is running in QOOL, take this time to deepen your understanding of IR spectroscopy and how it relates to your chosen molecule. Reflect on the following questions to prepare for analyzing your results:

   - How might factors such as **hydrogen bonding** or **conjugation** affect the positions and intensities of these absorption peaks?  
   - What strategies will you use to **assign the observed absorption peaks** to specific bond vibrations in your molecule?  
   - How will you handle **overlapping peaks** or those that fall within the **fingerprint region (1500–500 cm⁻¹)**?  
   - In what ways does **molecular symmetry** and structure affect the IR spectrum?  
   - How do different **vibrational modes** (e.g., stretching vs. bending) manifest in the IR absorption patterns?

---

### 5. Analyzing the IR Spectrum

1. **Access the Results**  
   - Once the calculation is complete, open the IR spectrum generated by QOOL.

2. **Identify Absorption Peaks**  
   - Examine the spectrum to locate key absorption peaks.  
   - Record the wavenumbers (in cm⁻¹) of significant peaks.

3. **Assign Peaks to Functional Groups**  
   - Use IR spectroscopy reference charts to correlate observed peaks with specific bond vibrations and functional groups.

4. **Interpret the Spectrum**  
   - Analyze how the peaks correspond to the molecular structure of your molecule.  
   - Consider factors like **bond types**, **functional groups**, and **molecular symmetry**.

!!! success "SUBMIT YOUR IR SPECTRUM TABLE"
    **Example Table**: Methanol IR Spectrum  
    Prepare a table for each compound to record the observed peaks and their assignments.

<figure markdown="span">
  ![Example: Methanol IR Spectrum Key Peaks](https://dummyimage.com/600x400/){ width="300" }
  <figcaption>Example: Methanol IR Spectrum Key Peaks</figcaption>
</figure>

| Observed Wavenumber (cm⁻¹) | Assigned Vibration  | Functional Group |
|----------------------------|---------------------|------------------|
| ~3200–3400                | O–H Stretch         | Hydroxyl (OH)    |
| ~2950                      | C–H Stretch         | Alkyl (CH₃)      |
| ...                        | ...                 | ...              |

---

## Post Lab Questions

1. **Why is the O–H stretch in ethanol broad compared to other absorption peaks?**  
2. **How does hydrogen bonding influence the IR spectrum of ethanol?**  
3. **Explain why the C=O stretch in acetone appears as a strong, sharp peak.**  
4. **What factors affect the exact position of the carbonyl stretch in the IR spectrum?**  
5. **Identify the peaks associated with the aromatic C–H stretches in styrene.**  
6. **Discuss how conjugation in the aromatic ring affects the absorption frequencies.**  
7. **Compare the IR spectra of ethanol and acetone.** How do the spectra reflect differences in their functional groups?  
8. **What challenges might you face** when interpreting the IR spectrum of a molecule with multiple functional groups?  
9. **How can IR spectroscopy be used** in conjunction with other analytical techniques for structural determination?  
10. **Discuss the importance** of the fingerprint region (1500–500 cm⁻¹) in IR spectroscopy.

---


