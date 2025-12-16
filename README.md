# Surface Brightness Profile of a Galaxy

This repository contains a Jupyter Notebook that demonstrates how to compute and visualize the **surface brightness profile** of a galaxy from imaging data using Python. The notebook is intended to be **educational, reproducible, and accessible** to students and early researchers in astronomy and astrophysics.

---

## What this notebook does

The notebook walks through a complete, minimal workflow for surface photometry:

1. Load astronomical image data (FITS format)
2. Estimate and subtract the background
3. Determine the galaxy center using a 2D centroiding method
4. Construct concentric circular annuli around the galaxy center
5. Measure the mean flux in each annulus
6. Convert these measurements into a **radial surface brightness profile**
7. Visualize the result using Matplotlib

The final output is a plot showing how the galaxy’s brightness varies with radius.

---

## Scientific context

The **surface brightness profile** is a fundamental diagnostic tool in observational astronomy. It is widely used to:

* Study galaxy structure (bulge, disk, halo)
* Compare observations with theoretical models
* Fit analytic profiles (e.g., exponential disk, Sérsic profile)
* Investigate galaxy evolution

This notebook focuses on the *methodology*, not on fitting or interpretation, making it suitable as a starting point for further analysis.

---

## Requirements

The notebook uses standard scientific Python libraries:

* `numpy`
* `matplotlib`
* `astropy`
* `photutils`

You can install the required packages using:

```bash
pip install numpy matplotlib astropy photutils
```

---

## How to use

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   ```

2. Open the notebook:

   ```bash
   jupyter notebook surface_brightness_profile.ipynb
   ```

3. Replace the example FITS file with your own galaxy image if desired.

4. Run the cells sequentially to reproduce the analysis.

All steps are written explicitly to make the workflow easy to follow and modify.

---

## Who this is for

This notebook is designed for:

* Undergraduate and MSc physics / astronomy students
* Beginners learning astronomical data analysis
* Anyone new to surface photometry

No prior experience with `photutils` is assumed.

---

## Limitations and notes

* The analysis assumes **circular symmetry** (circular annuli)
* Effects such as PSF correction, inclination, and extinction are not included
* The surface brightness is shown in instrumental units unless calibrated separately

These simplifications are intentional for clarity and learning purposes.

---

## License

This project is released for educational and academic use. You are free to reuse and modify the code with appropriate attribution.

---

## Acknowledgments

This notebook uses open-source tools from the Astropy and Photutils ecosystems. Their documentation and examples were invaluable in shaping this workflow.

---

If you find this notebook useful, feel free to star the repository or adapt it for your own projects.
