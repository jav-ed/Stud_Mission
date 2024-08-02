# Development of a Module for Mission Analysis in Gradient-Based Aerodynamic Shape Optimization

## About This Repository

This repository contains the complete LaTeX source, figures, and compiled [PDF](100_Compiled/main.pdf) of my studienarbeit (student research project), submitted on 19.08.2021 to the Technische Universität Braunschweig, Department of Mechanical Engineering, Chair for Overall Aircraft Design, in cooperation with the German Aerospace Center (DLR).

![Gradient Model 28](2_Figures/0_Deco/grad_Model_28-1.png)

## Thesis Overview

This studienarbeit focuses on the development of a module for mission analysis within a gradient-based aerodynamic shape optimization process. The work contributes to the field of aeronautical engineering and computational design optimization.

## Key Achievements

* Developed a lightweight Python tool (missioninformer) from scratch for calculating total fuel mass and its gradients for user-defined flight missions
* Implemented physics-based equations for cruise segment analysis and integrated empirical fuel fractions for other flight phases
* Conducted extensive investigations on surrogate models (RBF, Kriging, TPS) to optimize interpolation accuracy and execution time
* Performed in-depth analysis of ODE solvers, comparing analytical and numerical solutions to ensure high accuracy in fuel mass calculations
* Implemented and optimized gradient calculations using central differencing scheme, including a detailed step-size study
* Integrated mass snowball effects through fix-point iterations for more realistic fuel consumption estimates
* Explored and compared various surrogate model options, conducting computationally intensive model selection studies
* Optimized the tool's performance, achieving runtime between 50 to 800 seconds for two-mission calculations including gradient computation
* Designed the tool to be easily integrated into gradient-based and gradient-free optimization workflows
* Contributed to environmental efforts in aviation by creating a tool to help reduce aircraft fuel consumption and emissions


## Repository Structure

- Inshallah [Final compiled PDF](100_Compiled/main.pdf)
- `100_Compiled/`: Contains log, auxiliary files, and the compiled PDF itself
- `1_Latex_Files/`: LaTeX source files
- `2_Figures/`: Figures and images used in the thesis
- `3_Bibtex/`: Bibliography files
- `main.tex`: The main LaTeX file for the thesis
- `license.md`: License information for this project
- `README.md`: This file, providing an overview of the repository

## Compilation Note

This project uses TikZ diagrams generated with pyxdsm. To compile the thesis correctly, you need to:

1. Create a virtual environment and activate it
2. Install pyxdsm: `pip install pyxdsm`
3. Locate the `diagram_styles.tex` file:
   ```
   find /path/to/your/virtualenv -name diagram_styles.tex
   ```
4. Replace the following line in the relevant .tex files:
    ```
    \input{/home/jav/Progs/Virt_Env/writing/lib/python3.12/site-packages/pyxdsm/diagram_styles.tex}
    ```
with the actual path to the `diagram_styles.tex` file on your system.

## Important Notes

1. The PDF file in `100_Compiled/` is the original, unmodified version as submitted.
2. This repository can be used as a template for similar projects.
3. We all learn and grow. I acknowledge that mistakes were made in the past, and inshallah, I will continue to learn from future experiences. Only the Acknowledgement section has been slightly modified in this version. This modification does not affect the academic content of the thesis.

## License

Please refer to the `license.md` file in this repository for detailed licensing information.


## Contact

For more information or to get in touch, please visit my website: [javedab.com](https://javedab.com)

## Note on README Creation

This README was created with the assistance of an AI large language model, specifically the Claude 3.5 Sonnet model. While the content accurately reflects the thesis and repository structure, the wording and organization were enhanced through AI collaboration.

---

Feel free to explore this repository and use it as a reference for your own work. If you have any questions or feedback, please don't hesitate to reach out through the contact information provided above.