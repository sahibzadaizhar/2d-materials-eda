## Exploratory Data Analysis of 2D van der Waals Heterostructures

### About This Project

This repository contains an exploratory data analysis (EDA) of four NbX₂-HfY₂ (X=Se, Te; Y=S, Se) van der Waals heterostructures. The data comes from my published first-principles DFT calculations.

The main goal was to understand how mechanical strain affects the electronic properties of these materials, specifically the **n-type Schottky barrier height (Φ_Bn)**. A barrier close to zero is what we want for an Ohmic contact, which is essential for low-resistance nanoelectronic devices.

I wanted to see which of the four heterostructures could be tuned to an Ohmic contact with the least amount of strain, and how the work function and barrier heights behave under different strain conditions.

### The Data

The data is taken from **Table 3** of my published manuscript. It includes strain-dependent properties for four heterostructures:

1.  NbSe₂-HfS₂
2.  NbTe₂-HfS₂
3.  NbSe₂-HfSe₂
4.  NbTe₂-HfSe₂

The properties I analyzed are:
- **Strain (%)**: The applied mechanical strain (from -10% to +10%).
- **Work Function (eV)**: The energy required to remove an electron from the surface.
- **n-type Schottky Barrier (eV)**: The barrier for electrons.
- **p-type Schottky Barrier (eV)**: The barrier for holes.

### Tools I Used

I used Python for this analysis. The main libraries are:
- **Pandas**: For loading and organizing the data.
- **NumPy**: For numerical operations.
- **Matplotlib** and **Seaborn**: For creating static plots.
- **Plotly**: For making an interactive plot.

### What I Found

After running the analysis, here are the main takeaways:

1.  **Strain is a powerful tool.** For **NbSe₂-HfS₂**, I found that an Ohmic contact (barrier ≈ 0) is achieved at around **8% tensile strain**. This is a promising result for device design.
2.  **Not all materials behave the same.** The selenide-based heterostructures (NbSe₂-HfSe₂) show a different trend than the sulfide-based ones. This means material selection is critical.
3.  **At equilibrium (0% strain), NbSe₂-HfS₂ has the lowest barrier** (~0.75 eV). It is the most promising candidate even before strain is applied.

### The Figures

The notebook contains six figures that I used to explore the data:

- **Figure 1**: A line plot showing how the n-type Schottky barrier changes with strain for all four materials.
- **Figure 2**: A correlation heatmap showing how the different properties are related to each other.
- **Figure 3**: An interactive scatter plot (Plotly) of strain vs. work function.
- **Figure 4**: A box plot showing the distribution of the n-type barrier for each material.
- **Figure 5**: A violin plot showing the distribution of the work function for each material.
- **Figure 6**: A bar chart comparing the n-type barrier at 0% strain.

### How to Use This Repository

If you want to run this notebook yourself, follow these steps:
1.  Clone the repository:
    ```bash
    git clone https://github.com/sahibzadaizhar/2d-materials-eda.git
Open the Jupyter Notebook:
jupyter notebook My_Project.ipynb
Run the cells to reproduce the analysis and the figures.

### About Me
I am a computational condensed matter physicist. My work focuses on using DFT to understand and design 2D materials for nanoelectronic and optoelectronic applications. This project is part of my ongoing research on strain-engineered van der Waals heterostructures.

ResearchGate: https://www.researchgate.net/profile/Sahibzada-Izhar-Hussain-Bacha-2

Email: sahibzadaibh@gmail.com
